# Avoid Instantiation For Get Class

```
public class AvoidInstantiationForGetClassRejected
{
	public void getClass() 
	{
		Class c = (new Avoid_instantiation_for_getClass_violation()).getClass();
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class AvoidInstantiationForGetClassResolved
{
	public void getClass()
    {
    	Class c = Avoid_instantiation_for_getClass_correction.class; 
    }
}
```