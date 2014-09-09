#Constant Expressions In Loops

```
public class ConstantExpressionsInLoopsRejected
{
	public static final boolean TRUE= true;
    public static final boolean FALSE= false;
    public static final int VALUE = 7;
     
    public void loop()
    {
      int[] x = new int[10];
      int j = 0;
      
      for(int i = 0; i < 10; i++)
      {
        x[0] = 1 + (VALUE + 100);
        for(j = 0; TRUE || FALSE ; )
        ;;
     }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class ConstantExpressionsInLoopsResolved
{
	 public void myMethod()
     {
       int[] x = new int[10];
       int j = 0;
      
       x[0] = 1 + (FOO + 100);
       for(int i=0; i<10; i++)
       {
         for(j=0; TRUE ; ) 
         ;;
       }
    }
}
```