Use PreparedStatement
===============

```
public class UsePreparedStatementRejected
{
	public void method(Connection connection) throws Exception
    {
        Statement statement = connection.createStatement();
        for (int i = 0; i < empCount; i++)
        {
            String sQry = "SELECT * FROM employee WHERE id = " + i;
            ResultSet rs = stmt.execute(sQry);
            
            ...
        }
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class UsePreparedStatementResolved
{
	public void method(Connection connection) throws Exception
    {
        String sQry = "SELECT * FROM employee WHERE id = ?";
        PreparedStatement preparedStatement = connection.prepareStatement(sQry);
        for (int i = 0; i < empCount; i++)
        {
            preparedStatement.setString(1,""+i);
            ResultSet rs = preparedStatement.executeQuery();
            //...
        }
    }
}
```
