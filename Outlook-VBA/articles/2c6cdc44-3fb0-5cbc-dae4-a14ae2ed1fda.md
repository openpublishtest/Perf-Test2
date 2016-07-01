
# TaskRequestDeclineItem.GetConversation Method (Outlook)

Obtains a  **[Conversation](2705d38a-ebc0-e5a7-208b-ffe1f5446b1b.md)** object that represents the conversation to which this item belongs.


## Syntax

 _expression_ . **GetConversation**

 _expression_ A variable that represents a **[TaskRequestDeclineItem](e842c7c0-7943-9219-329b-30b892ab99b0.md)** object.


### Return Value

A  **Conversation** object that represents the conversation to which this item belongs.


## Remarks

 **GetConversation** returns **Null** ( **Nothing** in Visual Basic) if no conversation exists for the item. No conversation exists for an item in the following scenarios:


- The item has not been saved. An item can be saved programmatically, by user action, or by auto-save.
    
- For an item that can be sent (for example, a mail item, appointment item, or contact item), the item has not been sent.
    
- Conversations have been disabled through the Windows registry.
    
- The store does not support Conversation view (for example, Outlook is running in classic online mode against a version of Microsoft Exchange earlier than Microsoft Exchange Server 2010). Use the  **[IsConversationEnabled](ce333881-a5f3-2115-0ae4-296d15c4bead.md)** property of the **[Store](1eb22fe9-8849-7476-5388-2515b48591b9.md)** object to determine whether the store supports Conversation view.
    



## See also


#### Concepts


[TaskRequestDeclineItem Object](e842c7c0-7943-9219-329b-30b892ab99b0.md)
#### Other resources


[TaskRequestDeclineItem Object Members](3de31d0d-2444-876c-5d4d-1192851301af.md)
