Single Quotes When Concatenating Character To String
============

```
public class SingleQuotesWhenConcatenatingCharacterToStringRejected
{
	public void concatenating{
    {
        String str = "Dat";
        str += "e";
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class SingleQuotesWhenConcatenatingCharacterToStringResolved
{
	public void concatenating{
        {
            String str = "Dat";
            str += 'e';
        }
}
```
