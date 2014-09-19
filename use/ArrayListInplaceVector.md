ArrayList inplace of Vector
======

```
   public class ArrayListInplaceOfVectorRejected
   {
       final int SIZE = 10;
       private Vector v = new Vector(SIZE);		
        
        public int size()
        {
     	 	return v.size();
     	}
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class ArrayListInplaceOfVectorResolved
   {
       final int SIZE = 10;
       private List list = new ArrayList(SIZE);		
        
        public Integer size()
        {
            return list.size();
        }
   }
```

