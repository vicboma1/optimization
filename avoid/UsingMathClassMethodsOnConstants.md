#Using math class methods on constants

```
public class UsingMathClassMethodsOnConstantsRejected
{
	public void foo() 
	{
		final double aux = Math.abs(1.5); 
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class UsingMathClassMethodsOnConstantsResolved
{
	public void foo() 
	{
		double a = 1.5;
	}
}
```



