Loop Invariant Code Motion
=======

```
public class LoopInvariantCodeMotionRejected
{     
    public Integer method()
    {
        String name = "Victor";
        for(int i = 0; i < z; i++)
        {
           name += name +"_"+ i;
        }
     }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class LoopInvariantCodeMotionResolved
{
	 public void method()
     {
        String name = "Victor";
        name+="_";
        for(int i = 0; i < z; i++)
        {
           name += name + i;
        }
    }
}
```