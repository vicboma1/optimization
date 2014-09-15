Method Final
=========

```
public class MethodFinalRejected
{
    private String _uid;
     
	public String UID{
    {
        return _uid;
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class MethodFinalResolved
{
	private String _uid;
         
    public final String UID{
    {
        return _uid;
    }
}
```
