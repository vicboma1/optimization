#Creating thread without run method

```
public class CreatingThreadWithoutRunMethodRejected
{
	public void method() 
	{
		new Thread().start(); 
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class CreatingThreadWithoutRunMethodResolved
{
	public void method(Runnable runnable) throws Exception
     {
     	new Thread(runnable).start();  
     }
}
```