#Duplication Code

```
public class DuplicationCodeRejected
{
	public void get(int value)
    	{
    		int x = value;
    
    		if(x > 1)
    		{				
    			int j = i + 10;
    			int k = j * 2;
    			System.out.println(k);			
    		}
    		else if( x < 10 )
    		{				
    			int j = i + 10;
    			int k = j * 2;
    			System.out.println(k);			
    		}
    		else {
    		}
    	}
    		
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class DuplicationCodeResolved
{
	public void IntegerToString()
    {
     	public void get(int value)
        {
            int x = value;
            int j = i + 10;
            int k = j * 2;
    
            if(x > 1)
              System.out.println(k);			
            else if( x < 10 )
                System.out.println(k);			
            else {
            }
        }
     }
}
```