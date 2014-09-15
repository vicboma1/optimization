Passing Primitive double To Double Constructor
=========

```
public class PassingPrimitivedoubleToDoubleConstructorRejected
{
    public void method() 
    {
        Double i = new Double(3.0);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitivedoubleToDoubleConstructorResolved
{
    public void method()
    {
        Double i = Double.valueOf(3.0);
         ...
    }
}
   ```