Lazy Initialization
=========

```
public class LazyInitializationRejected
{
	private Singleton instance = new Singleton();  
     
	...
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class LazyInitializationResolved
{
	private Singleton instance;  
    	
    public Singleton getInstance()
    {
        if(instance == null)
            instance  =  new Singleton();
        return instance;
    }
}
```
