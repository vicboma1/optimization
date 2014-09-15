JDBC Resources
========

```
public class JDBCResourcesRejected
{
    public void method() 
    {
        Connection connection = null;
        Statement statement = null;
        ResultSet resultSet = null;
        
        try
        {
            connection = DriverManager.getConnection(url);
            statement = conn.createStatement();
            resultSet = stmt.executeQuery(query);
            
            resultSet.close();	
            statement.close();	
            connection.close();			
            
        }
        catch (Exception e)
        {
        }
        finally
        {
        
        
        }
    }
}   
```
![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   
public class JDBCResourcesResolved
{
    public void method()
    {
        Connection connection = null;
        Statement statement = null;
        ResultSet resultSet = null;
                
        try
        {
            connection = DriverManager.getConnection(url);
            statement = conn.createStatement();
            resultSet = stmt.executeQuery(query);       
            
        }
        catch (Exception e)
        {
            e.printStackTrace();
        }
        finally
        {
            try
            {
                resultSet.close();	
                statement.close();	
                connection.close();	
            }
            catch (Exception e)
            {
            }
        }
    }
}
   ```