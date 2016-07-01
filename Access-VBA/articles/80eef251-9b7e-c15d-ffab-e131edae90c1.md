
# SubForm.Tag Property (Access)

Stores extra information about a form, report, section, or control needed by a Microsoft Access application. Read/write  **String**.


## Syntax

 _expression_. **Tag**

 _expression_ A variable that represents a **SubForm** object.


## Remarks

You can enter a string expression up to 2048 characters long. The default setting is a zero-length string (" ").

Unlike other properties, the  **Tag** property setting doesn't affect any of an object's attributes.

You can use this property to assign an identification string to an object without affecting any of its other property settings or causing other side effects. The  **Tag** property is useful when you need to check the identity of a form, report, section, or control that is passed as a variable to a procedure.


## Example

The following example uses the  **Tag** property to display custom messages about controls on a form. When a control has the focus, descriptive text is displayed in a label control called `lblMessage`. You specify the text for the message by setting the  **Tag** property for each control to a short text string. When a control receives the focus, its **Tag** property is assigned to the label control's **Caption** property. This example displays the descriptive text for a text box named `txtDescription` and a command button named `cmdButton` on a form.


```
Sub Form_Load() 
 Dim frmMessageForm As Form 
 
 Set frmMessageForm = Forms!Form1 
 
 frmMessageForm!lblMessage.Caption = "" ' Clear text. 
 frmMessageForm!txtDescription.Tag = "Help text for the text box." 
 frmMessageForm!cmdButton.Tag = "Help text for the command button." 
End Sub 
 
Sub txtDescription_GotFocus() 
 ' Tag property setting as caption. 
 Me!lblMessage.Caption = Me!txtDescription.Tag 
End Sub 
 
Sub txtDescription_LostFocus() 
 Me!lblMessage.Caption = "" 
End Sub 
 
Sub cmdButton_GotFocus() 
 ' Tag property setting as caption. 
 Me!lblMessage.Caption = Me!cmdButton.Tag 
End Sub 
 
Sub cmdButton_LostFocus() 
 Me.lblMessage.Caption = " " 
End Sub
```


## See also


#### Concepts


[SubForm Object](60f961fa-dcf4-e1d1-8c50-9e88963f9dec.md)
#### Other resources


[SubForm Object Members](328e74d8-0418-968f-faca-3e1b34139f48.md)