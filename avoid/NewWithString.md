New With String
=======

```
public class NewWithStringRejected
{
    public Integer method(String parameter) 
    {
       String str = new String(parameter);	
       return str.length();
    }
}

```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
public class NewWithStringResolved
{
     public Integer method(String parameter) 
    {
       String str = parameter;	
       return str.length();
    }
}
```