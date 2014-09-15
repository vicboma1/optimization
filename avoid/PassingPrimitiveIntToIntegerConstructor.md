Passing Primitive int To Integer Constructor
=========

```
public class PassingPrimitiveintToIntegerConstructorRejected
{
    public void method() 
    {
        Integer i = new Integer(3.0);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitiveIntToIntegerConstructorResolved
{
    public void method()
    {
        Integer i = Integer.valueOf(3.0);
         ...
    }
}
   ```