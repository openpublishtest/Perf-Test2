
# Column.Session Property (Outlook)

Returns the  **[NameSpace](f0dcaa19-07f5-5d42-a3bf-2e42b7885644.md)** object for the current session. Read-only.


## Syntax

 _expression_ . **Session**

 _expression_ A variable that represents a **Column** object.


## Remarks

The  **Session** property and the **[Application.GetNamespace](6175d0d9-5a61-ce45-35c0-b70895d757b3.md)** method can be used interchangeably to obtain the **NameSpace** object for the current session. Both members serve the same purpose. For example, the following statements perform the same function:


```
Set objNamespace = Application.GetNamespace("MAPI") 
```


```
Set objSession = Application.Session
```


## See also


#### Concepts


[Column Object](b7eb6916-2d80-57c3-2077-47a2a4c73185.md)
#### Other resources


[Column Object Members](c9b724b2-49e3-8cd5-95c7-0e4ea423df46.md)
