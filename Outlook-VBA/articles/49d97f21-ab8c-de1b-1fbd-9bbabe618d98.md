
# Inspector.Display Method (Outlook)

Displays a new  **[Inspector](d7384756-669c-0549-1032-c3b864187994.md)** object for the item.


## Syntax

 _expression_ . **Display**( **_Modal_** )

 _expression_ A variable that represents an **Inspector** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Modal_|Optional| **Variant**| **True** to make the window modal. The default value is **False** .|

## Remarks

The  **Display** method is supported for explorer and inspector windows for the sake of backward compatibility. To activate an explorer or inspector window, use the **[Activate](d7784df0-b595-6f5a-2195-27ad021db6de.md)** method.

If you attempt to open an "unsafe" file system object (or "freedoc" file) by using the Microsoft Outlook object model, you receive the  **E_FAIL** return code in the C or C++ programming languages. In Outlook 2000 and earlier, you could open an "unsafe" file system object by using the **Display** method.


## See also


#### Concepts


[Inspector Object](d7384756-669c-0549-1032-c3b864187994.md)
#### Other resources


[Inspector Object Members](acd3e13f-4727-7966-d2a5-a95e4528425c.md)
