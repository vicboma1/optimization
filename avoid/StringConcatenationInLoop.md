String Concatenation In Loop
=============

```
   public class StringConcatenationInLoopRejected
   {
        public void method() 
        {
            String result = "";
            for (int i = 0; i < 100; i++) 
                result += i+" /n";
        }
   }
   
```   
![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class StringConcatenationInLoopResolved    // synchronous
   {
     	public void method()
        {
        	String result = "";
            StringBuffer buffer = new StringBuffer();
            for (int i = 0; i < 100; i++) 
                buffer.append(i+" /n");	
                		
            result = buffer.toString();				       
        }
   }
```
OR

```
 public class StringConcatenationInLoopResolved 
   {
     	public void method()
        {
        	String result = "";
            StringBuilder builder = new StringBuilder();
            for (int i = 0; i < 100; i++) 
                builder.append(i+" /n");	
                		
            result = builder.toString();				       
        }
   }
```

