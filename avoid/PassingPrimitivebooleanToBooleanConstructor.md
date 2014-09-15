Passing Primitive boolean To Boolean Constructor
=========

```
public class PassingPrimitivebooleanToBooleanConstructorRejected
{
    public void method() 
    {
        Boolean i = new Boolean(true);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitivebooleanToBooleanConstructorResolved
{
    public void method()
    {
        Boolean i = Boolean.true;
         ...
    }
}
   ```