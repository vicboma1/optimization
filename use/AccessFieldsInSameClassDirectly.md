Access Fields In Same Class Directly
======

```
public class AccessFieldsInSameClassDirectlyRejected
{
    final boolean modified = false;
    
    public boolean isModified()
    {
        return modified;
    }

    public void save()
    {
        if (isModified())
        {
            ...
        }
    }
}
   ```
   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
   ```
   
public class AccessFieldsInSameClassDirectlyResolved
{
    final boolean modified = false;
   	
    public boolean isModified()
    {
        return modified;
    }

    public void save()
    {
        if (modified) //correction
        {
            ...
        }
    }
}
   ```