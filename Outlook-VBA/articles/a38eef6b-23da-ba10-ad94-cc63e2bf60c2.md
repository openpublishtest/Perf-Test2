
# RemoteItem.Write Event (Outlook)

Occurs when an instance of the parent object is saved, either explicitly (for example, using the  **[Save](0f4e57ab-388c-7ba1-c6b8-f14bfc0ac73c.md)** or **[SaveAs](1c2c7b68-5239-05f8-4291-d2584fe95194.md)** methods) or implicitly (for example, in response to a prompt when closing the item's inspector).


## Syntax

 _expression_ . **Write**( **_Cancel_** )

 _expression_ A variable that represents a **RemoteItem** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Cancel_|Required| **Boolean**| (Not used in VBScript). **False** when the event occurs. If the event procedure sets this argument to **True** , the save operation is not completed.|

## Remarks

In Microsoft Visual Basic Scripting Edition (VBScript), if you set the return value of this function to  **False** , the save operation is not completed.


## See also


#### Concepts


[RemoteItem Object](6302aaff-cdcf-4d86-60f1-4bed15540d9f.md)
#### Other resources


[RemoteItem Object Members](15c0872e-88cc-9b9b-c31e-c15d6971e6e0.md)
