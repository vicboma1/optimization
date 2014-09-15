Stream
=======


```
public class StreamRejected
{
	public void method(java.io.File f) throws IOException
    {
        FileInputStream fileInputStream = null;
        try
        {
            fileInputStream = new java.io.FileInputStream(f);		//Violation
            fileInputStream.read ();
        }
        catch (java.io.FileNotFoundException e1)
        {
            System.out.println("Exception : File not found");
        }
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class StreamResolved
{
	public void method(java.io.File f) throws IOException
    {
        FileInputStream fileInputStream = null;
        try
        {
            fileInputStream = new java.io.FileInputStream(f);
            fileInputStream.read ();			
        }
        catch (java.io.FileNotFoundException e1)
        {
            System.out.println("Exception : File not found");
        }
        finally
        {
            fileInputStream.close ();
        }
        
    }
}
```
