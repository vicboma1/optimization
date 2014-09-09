#Use String length to compare empty string variables

```
public class UseStringLengthToCompareEmptyStringVariablesRejected
{
	public boolean isEmpty(String str)
	{
		return str.equals("");
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```
public class UseStringLengthToCompareEmptyStringVariablesResolved
{
	public boolean isEmpty(String str)
	{
		return str.length() == 0;	
	}
}
```


