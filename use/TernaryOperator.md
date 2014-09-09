#Ternary operator

```
public class TernaryOperatorRejected
{
	public void isValid() 
	{
	    public Boolean test(String value)
        {
            if(value.equals("isValid"))
                return true;	
            else
                return false;
        }
	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class TernaryOperatorResolved
{
	public Boolean test(String value)
    {
        return value.equals("isValid");
    }
}
```