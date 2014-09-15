Using MessageFormat
=======

```
public class UsingMessageFormatRejected
{
	public void method() 
	{
		final int total = 1000;
        List<Integer> store = new ArrayList();
        MessageFormat Messageformat = new MessageFormat("The square of {0,number,#} is {1,number,#}");
        for (int i = 1; i <= total; i++)
        {
            store.set(0,new Integer(i));
            store.set(1,new Integer(i * i));
            String str = Messageformat.format(store);
            System.out.println(srt);
        }
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class UsingMessageFormatResolved
{
	public void method() 
	{
		final int total = 1000;
        String str;
        for (int i = 1; i <= N; i++)
        {
            str = "The square of " + i + " is " + (i * i);
            System.out.println(s);
        }
	}
}
```



