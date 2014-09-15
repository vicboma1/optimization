Boolean Operators
======

BooleanOperators

```
   public class BooleanOperatorsRejected
   {
        public void method(Boolean operation) 
        {
            if(operation.equals("true) | operation.equals("false)
                System.out.print("Operation valid);
        }
   }
   
```   
   ![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)
   
```
   public class BooleanOperatorsResolved
   {
     	public void method()
        {
        	 public void method(Boolean operation) 
            {
                if(operation.equals("true) ||  operation.equals("false)
                    System.out.print("Operation valid);
            }
        }
   }
```