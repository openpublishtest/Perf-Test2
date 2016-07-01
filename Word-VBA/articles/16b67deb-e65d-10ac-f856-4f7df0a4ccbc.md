
# View.ShowFirstLineOnly Property (Word)

 **True** if only the first line of body text is shown in outline view. Read/write **Boolean** .


## Syntax

 _expression_ . **ShowFirstLineOnly**

 _expression_ An expression that returns a **[View](8bf5b26b-14c0-1985-65b2-3e034360baeb.md)** object.


## Remarks

This property generates an error if the view isn't outline or master document view.


## Example

This example switches the active window to outline view and hides all but the first line of body text.


```vb
With ActiveDocument.ActiveWindow.View 
 .Type = wdOutlineView 
 .ShowFirstLineOnly = True 
End With
```


## See also


#### Concepts


[View Object](8bf5b26b-14c0-1985-65b2-3e034360baeb.md)
#### Other resources


[View Object Members](b7d2bd4e-c96d-3b8f-98a0-57c145f9aa42.md)
