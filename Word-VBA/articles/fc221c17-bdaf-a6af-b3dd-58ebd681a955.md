
# Axis.HasTitle Property (Word)

 **True** if the axis or chart has a visible title. Read/write **Boolean** .


## Syntax

 _expression_ . **HasTitle**

 _expression_ A variable that represents an **[Axis](3a7ad7d8-d397-a79a-eb6a-a5f0822cbe5d.md)** object.


## Remarks

An axis title is represented by an  **[AxisTitle](ec746a05-40df-95cc-c017-40ef150504cf.md)** object.


## Example

The following example adds an axis label to the category axis for the first chart in the active document.


```vb
With ActiveDocument.InlineShapes(1) 
 If .HasChart Then 
 With .Chart.Axis(xlCategory) 
 .HasTitle = True 
 .AxisTitle.Text = "July Sales" 
 End With 
 End If 
End With
```


## See also


#### Concepts


[Axis Object](3a7ad7d8-d397-a79a-eb6a-a5f0822cbe5d.md)
#### Other resources


[Axis Object Members](44fa1b67-2a56-3d92-cb63-4144e1bb7282.md)
