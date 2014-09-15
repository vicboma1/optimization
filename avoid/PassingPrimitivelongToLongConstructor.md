Passing Primitive long To Long Constructor
=========

```
public class PassingPrimitivelongToLongConstructorRejected
{
    public void method() 
    {
        Long i = new Long(3L);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitivelongToLongConstructorResolved
{
    public void method()
    {
        Long i = Long.valueOf(3L);
         ...
    }
}
   ```