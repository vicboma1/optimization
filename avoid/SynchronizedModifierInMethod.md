#Synchronized modifier in method

```
public class SynchronizedModifierInMethodRejected
{
	public synchronized void syncSetMethod(String name) throws IOException
	{
    	...
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class SynchronizedModifierInMethodResolved
{
	public void syncSetMethod(String name) throws IOException
    {
        Synchronized(this){
           ...
        }
    }
}
```

