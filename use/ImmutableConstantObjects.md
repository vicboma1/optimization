#Immutable Constant Objects

```
public class ImmutableConstantObjectsRejected
{
  protected Object[] getObjects() 
  {
    return new Object[0];  
  }
 
  public static Integer convertToInt(String s) 
  {
      if (s == null || s.length() == 0)
        return new Integer(-1); 
      else 
          return new Integer(s);
  }
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```
public class ImmutableConstantObjectsResolved
{
   private static final Object[] NO_OBJECTS = new Object[0];
   private static final Integer INT_N1 = new Integer(-1);
  
   protected Object[] getObjects() 
   {
     return NO_OBJECTS;
   }
     
   public static Integer convertToIn(String s) 
   {
     if (s == null || s.length() == 0)
        return INT_N1;
     else
        return new Integer(s);
    }
}
```