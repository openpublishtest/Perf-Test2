
# Report.OnActivate Property (Access)

Sets or returns the value of the  **On Activate** box in the **Properties** window of a form or report. Read/write **String**.


## Syntax

 _expression_. **OnActivate**

 _expression_ A variable that represents a **Report** object.


## Remarks

This property is helpful for programmatically changing the action Microsoft Access takes when an event is triggered. For example, between event calls you may want to change an expression's parameters, or switch from an event procedure to an expression or macro, depending on the circumstances under which the event was triggered.

The  **Activate** event occurs when the form or report receives the focus and becomes the active window.

The  **OnActivate** value will be one of the following, depending on the selection chosen in the **Choose Builder** window (accessed by clicking the **Build** button next to the **On Activate** box in the object's **Properties** window):


- If Expression Builder is chosen, the value will be "= _expression_", where  _expression_ is the expression from the Expression Builder window.
    
- If Macro Builder is chosen, the value is the name of the macro. 
    
- If Code Builder is chosen, the value will be "[Event Procedure]". 
    
If the  **On Activate** box is blank, the property value is an empty string.


## Example

The following example associates the  **Activate** event with the macro "Activate_Macro" for the "Order Entry" form.


```
Forms("Order Entry").OnActivate = "Activate_Macro"
```


## See also


#### Concepts


[Report Object](6f77c1b4-a9ce-7caa-204c-fe0755c6f9df.md)
#### Other resources


[Report Object Members](73370a33-1ca0-da4d-9e36-88011bc2b93e.md)