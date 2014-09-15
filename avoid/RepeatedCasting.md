Repeated Casting
=============


```
public class RepeatedCastingRejected
{
	public void method(Vehicle vehicle)
    {
        ((Vehicle) vehicle).setName("");		
        ((Vehicle) vehicle).setTurbo(false);	
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```

public class RepeatedCastingResolved
{
	public void method(Vehicle vehicle)
    { 
        final Vehicle car = (TextField) Vehicle;
        car.setName("");		
        car.setTurbo(false);	
    }
}
```

