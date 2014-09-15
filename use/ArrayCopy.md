System Array Copy
======

```
   public class ArrayCopyRejected
   {
        public static Integer[] copyArray (Integer[] array)
        {
            int length = array.length;
            int[] copy = new int [length];
            for(int i=0;i<length;i++)
                copy [i] = array[i];		
        
            return copy;
        }
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class ArrayCopyResolved
   {
     	public int[] copyArray (int[] array)
        {
            final int ZERO = 0;
            final int length = array.length;
            int[] copy = new int [length];
            System.arraycopy(array, ZERO, copy, ZERO, length);		
            return copy;
        }
   }
```

