Buffered IO
============

```
public class BufferedIORejected
{
	public static void copy(String from, String to) throws IOException
    {
        final int NEGATIVE = -1;
        InputStream in = null;
        OutputStream out = null;
       
        try
        {
            in = new FileInputStream(from);	
            out = new FileOutputStream(to);		
           
            while (true)
            {
                int data = in.read();
                if (data == NEGATIVE)
                 break;
                
                out.write(data);
            }
                in.close();
                out.close();
        }
       finally
       {
           if (in != null)
              in.close();
             
           if (out != null)
              out.close();
         
       }
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class BufferedIOResolved
{
	public static void copy(String from, String to) throws IOException
    {
        final int NEGATIVE = -1;
        InputStream in = null;
        OutputStream out = null;
        
        try
    	{
    		in = new BufferedInputStream(new FileInputStream(from));		// synchronization
    	    out = new BufferedOutputStream(new FileOutputStream(to));		// synchronization
    	
    	    while (true)
            {
                int data = in.read();
                if (data == NEGATIVE)
                    break;
            
                out.write(data);
    	    }
        }
    	finally
    	{
    	 	if (in != null)
    	  	   in.close();
    	      
    	    if (out != null)
    	       out.close();
    	  
        }
    }
}
```
