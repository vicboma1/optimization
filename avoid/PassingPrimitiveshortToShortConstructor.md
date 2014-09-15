Passing Primitive short To Short Constructor
=========

```
public class PassingPrimitiveshortToShortConstructorRejected
{
    public void method() 
    {
        Short i = new Short(3.0);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitiveshortToShortConstructorResolved
{
    public void method()
    {
        Short i = Short.valueOf(3.0);
         ...
    }
}
   ```