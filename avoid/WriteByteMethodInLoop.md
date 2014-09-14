WriteByte Method in loop
================


```
public static void main(String args[])
{
    final int ZERO = 0;
    final int ONE = 1;
    final int TEN = 10;
    String strFileName = "C:\\demoWriteByte.java";
    try
    {
        java.io.FileOutputStream fos = new java.io.FileOutputStream(strFileName);
        java.io.DataOutputStream ds = new java.io.DataOutputStream(fos);

        int i = ZERO;
        while(i < TEN)
        {
            ds.writeByte(ONE);	// VIOLATION
            i++;
        }

        for(i=ZERO; i<TEN; i++)
        {
            ds.writeByte(ONE);	// VIOLATION
        }

        i = ZERO;

        do
        {
            ds.writeByte(ONE);	// VIOLATION
            i++;
        }
        while(i<TEN);
    }
    catch(java.io.IOException e)
    {
        e.printStackTrace();
    }
}
```

![](http://www.iconki.com/icons/Software-Applications/32x32-Applications-Basics/arrow_down_blue.png)

```
public static void main(String args[])
{
    final int ZERO = 0;
    final char ONE = '1';
    final int TEN = 10;

    String strFileName = "C:\\demo.java"; //$NON-NLS-1$
    byte bArr[] = new byte[10];

    try
    {
        java.io.FileOutputStream fos = new java.io.FileOutputStream(strFileName);
        java.io.DataOutputStream ds = new java.io.DataOutputStream(fos);

        int i = ZERO;
        while(i < TEN)
        {
            bArr[i] = ONE;
            i++;
        }

        ds.write(bArr, ZERO, bArr.length);	// CORRECTION
    }
    catch(java.io.IOException e)
    {
        e.printStackTrace();
    }
}
```



