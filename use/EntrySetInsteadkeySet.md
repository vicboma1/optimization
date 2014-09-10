#EntrySet Instead of keySet
```
public class EntrySetInsteadkeySetRejected
{
    public void iterator()
 	{
 		Map<Object,Object> map = new HashMap<Object,Object>();
 		Iterator it = map.keySet().iterator();
 		Object key = it.next();
 		Object v = map.get(key);		
  	}
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```
public class EntrySetInsteadkeySetResolved
{
    public void method()
    {
       Map<Object,Object> map = new HashMap();
       Set<Object> set = map.entrySet();
       Object keyValuePair = it.next();
     }

}
```