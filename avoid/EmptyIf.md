#Empty if

```
   public class EmptyIfRejected
   {
        public void foo() 
        {
            final int ZERO = 0;
            int i = 10;
            
            if (i < ZERO)		
            {
            }
            else 
                i = ZERO;
        }
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class EmptyIfResolved
   {
     	public void foo()
        {
        	final int ZERO = 0;
            int i = 10;
            i = ZERO; 
        }
   }
```