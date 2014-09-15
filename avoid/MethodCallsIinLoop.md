Method Calls In Loop
=========


```
public class MethodCallsInLoopRejected
{
    String str = "Hello World";
    for (int i = 0; i < str.length(); i++)		
    {
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class MethodCallsInLoopResolved
{
    public void IntegerToString()
    {
        String str = "Hello World";
        final int length = str.length();		
        for (int i = 0; i < length ; i++)
        {
           ...
        }
    }
}
   ```