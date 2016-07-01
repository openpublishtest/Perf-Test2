
# CommandBarPopup.Priority Property (Office)

Gets or sets the priority of a  **CommandBarPopup** control. Read/write.


## 


 **Note**  The use of CommandBars in some Microsoft Office applications has been superseded by the new ribbon component of the Microsoft Office Fluent user interface. For more information, search Help for the keyword "ribbon."


## Syntax

 _expression_. **Priority**

 _expression_ A variable that represents a **CommandBarPopup** object.


### Return Value

Integer


## Remarks

 A control's priority determines whether the control can be dropped from a docked command bar if the command bar controls can't fit in a single row. Controls that can't fit in a single row drop off command bars from right to left.


## Example

The following example sets the descriptive text and priority of a command bar popup.


```
Dim popControl As CommandBarPopup 
Set popControl = Application.CommandBars.FindControl _ 
(Type:=msoControlPopup, Tag:="Graphics") 
 
With popControl. 
            .DescriptionText = "Graphics Selection dialog" 
            .Priority = 5 
End With 

```


## See also


#### Concepts


[CommandBarPopup Object](a8ae06a3-1d7b-a531-91df-756fafee5314.md)
#### Other resources


[CommandBarPopup Object Members](8ec16deb-bb74-2871-d837-f706c7a58f2b.md)