
# ContactItem.BeforeAttachmentSave Event (Outlook)

Occurs just before an attachment is saved.


## Syntax

 _expression_ . **BeforeAttachmentSave**( **_Attachment_** , **_Cancel_** )

 _expression_ A variable that represents a **ContactItem** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Attachment_|Required| **[Attachment](3e11582b-ac90-0948-bc37-506570bb287b.md)**|The  **Attachment** to be saved.|
| _Cancel_|Required| **Boolean**|(Not used in VBScript).  **False** when the event occurs. If the event procedure sets this argument to **True** , the save operation is not completed and the attachment is not changed.|

## Remarks

This event corresponds to when attachments are saved to the messaging store. The  **BeforeAttachmentSave** event occurs just before an attachment is saved when an item is saved. If a user edits an attachment and then saves those changes, the **BeforeAttachmentSave** event will not occur at that time; instead it will occur when the item itself is later saved. It also does not occur when the attachment is saved on the hard disk using the **SaveAsFile** method.

In VBScript, if you set the return value of this function to  **False** , the save operation is cancelled and the attachment is not changed.


## See also


#### Concepts


[ContactItem Object](8e32093c-a678-f1fd-3f35-c2d8994d166f.md)
#### Other resources


[ContactItem Object Members](a8b13369-4c87-02aa-e62a-1f3067e559fa.md)
