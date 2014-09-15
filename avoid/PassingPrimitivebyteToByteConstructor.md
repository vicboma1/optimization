Passing Primitive byte To Byte Constructor
=========

```
public class PassingPrimitivebyteToByteConstructorRejected
{
    public void method() 
    {
        Byte i = new Byte(3);
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitivebyteToByteConstructorResolved
{
    public void method()
    {
        Byte i = Byte.valueOf(3);
         ...
    }
}
   ```