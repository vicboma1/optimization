Dispose SWT Control
=======


```
public class DisposeSWTControlRejected
{
	public void createControl(Composite cmp, int style)
    {
        Control ct = new Button(cmp, style);  
        
        ...
    }
    	
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class DisposeSWTControlResolved
{
	public void createControl(Composite cmp, int style)
    {
        Control ct = new Button(cmp, style);  
        
        ...
        ct.dispose();
    }
}
```