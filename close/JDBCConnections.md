JDBC Connections
========

```
public class JDBCConnections
{
    public void method() 
    {
        try
        {
            Connection conn = DriverManager.getConnection(url);		
                        
        }
        catch (Exception e)
        {
            e.printStackTrace();
        }
    }
}   
```
![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   
public class JDBCConnections
{
    public void method()
    {
        Connection conn = null;
        try
        {
            conn = DriverManager.getConnection(url);       
            ...
        }
        catch (Exception e)
        {
            e.printStackTrace();
        }
        finally
        {
            conn.close();
        }
    }
}
   ```