#New Integer ToString

```
public class NewIntegerToStringRejected
{
	public void IntegerToString() 
	{
		String str = new Integer(1).toString();
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class NewIntegerToStringResolved
{
	public void IntegerToString()
     {
     	String str = String.valueOf(1);  
     }
}
```