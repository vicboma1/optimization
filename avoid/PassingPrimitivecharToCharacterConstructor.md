Passing Primitive char To Character Constructor
=========

```
public class PassingPrimitivecharToCharacterConstructorRejected
{
    public void method() 
    {
        Character i = new Character('V');
        ...
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class PassingPrimitivecharToCharacterConstructorResolved
{
    public void method()
    {
        Character i = Character.valueOf('V');
         ...
    }
}
   ```