
# PropertyAccessor.Session Property (Outlook)

Returns the  **[NameSpace](f0dcaa19-07f5-5d42-a3bf-2e42b7885644.md)** object for the current session. Read-only.


## Syntax

 _expression_ . **Session**

 _expression_ A variable that represents a **PropertyAccessor** object.


## Remarks

The  **Session** property and the **[Application.GetNamespace](6175d0d9-5a61-ce45-35c0-b70895d757b3.md)** method can be used interchangeably to obtain the **[NameSpace](f0dcaa19-07f5-5d42-a3bf-2e42b7885644.md)** object for the current session. Both members serve the same purpose. For example, the following statements perform the same function:


```
Set objNamespace = Application.GetNamespace("MAPI") 
```


```
Set objSession = Application.Session
```


## See also


#### Concepts


[PropertyAccessor Object](2fc91e13-703c-3ec9-9066-ffee7144306c.md)
#### Other resources


[PropertyAccessor Object Members](3356e345-8878-0ed7-6783-1e49ddecc066.md)
