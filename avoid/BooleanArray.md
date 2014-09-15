Boolean Array
=======

```
public class BooleanArrayRejected
{     
    public void method()
    {
      boolean[] boleanArray = new boolean[]{
                true,
                false,
                false,
                true,
                true
           };
     }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class BooleanArrayResolved
{
	 public void method()
     {
         BitSet bitSet = new BitSet(5); 
      	 bitSet.set(0);
      	 bitSet.set(3);
      	 bitSet.set(4);
    }
}
```