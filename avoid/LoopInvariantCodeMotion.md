Loop Invariant Code Motion
=======

```
public class LoopInvariantCodeMotionRejected
{     
    public Integer method(Integer x, Integer y, Integer[] z)
    {
        for(int i = 0; i < z.length; i++)
        {
            z[i] = x * Math.abs(y);	
        }
     }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class LoopInvariantCodeMotionResolved
{
	public void method(Integer x, Integer y, Integer[] z)
    {
        final int result = x * Math.abs(y);	
        for(int i = 0; i < z.length; i++)
        {
            z[i] = result;
        }
    }
}
```