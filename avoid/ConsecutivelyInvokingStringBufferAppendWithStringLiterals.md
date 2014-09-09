#Consecutively Invoking String Buffer Append With String Literals

```
public class ConsecutivelyInvokingStringBufferAappendWithStringLiteralsRejected
{
	public void append() 
	{
	    StringBuffer buf = new StringBuffer();
     	buf.append("Hello").append(" ").append("World");
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class ConsecutivelyInvokingStringBufferAappendWithStringLiteralsResolved
{
	public void append() 
	{
		StringBuffer buf = new StringBuffer();
        buf.append("Hello World");
	}
}
```