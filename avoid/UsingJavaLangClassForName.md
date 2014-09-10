#Using Java Lang Class For Name

```
public class UsingJavaLangClassForNameRejected
{
	public void className(String name) 
	{
    	try {
	    	System.out.println(Class.forName(name).getName()); 
        }
        catch ( ClassNotFoundException e )
        {
             e.printStackTrace();
        }
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class UsingJavaLangClassForNameResolved
{
	public void className(String name) 
    {
        System.out.println(name.class.getName()); 
    }
}
```



