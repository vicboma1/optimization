Call to Thread Sleep
======

```
   public class CalltoThreadSleepRejected
   {
        public void mehotd(String url) throws SQLException
        {
           final long time = 1000L;
           Thread.sleep(time); 
       }
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class CalltoThreadSleepResolved
   {
     	public void method() throws SQLException
        {
            final long time = 1000L;
            this.wait(time); 
        }
   }
```