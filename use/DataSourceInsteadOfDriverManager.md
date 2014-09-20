DataSource instead of DriverManager
======

```
   public class DataSourceInsteadOfDriverManagerRejected
   {
        public void connection(String url) throws SQLException
        {
            Connection connection = DriverManager.getConnection(url); 
            ...
       }
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class DataSourceInsteadOfDriverManagerResolved
   {
     	public void connection() throws SQLException
        {
            Connection connection = ds.getConnection();
            ...        
        }
   }
```