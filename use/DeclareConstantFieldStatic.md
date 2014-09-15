Declare Constant Field Static
==============

```
public class DeclareConstantFieldStaticRejected
{
	final int MAX_INTEGER = Integer.MAX_VALUE;
    final int MIN_INTEGER = Integer.MIN_VALUE
    	
    ...
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class DeclareConstantFieldStaticResolved
{
	static final int MAX_INTEGER = Integer.MAX_VALUE;
    static final int MIN_INTEGER = Integer.MIN_VALUE
    
    ...
}
```
