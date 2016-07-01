
# Document.GridDistanceHorizontal Property (Word)

Returns or sets a  **Single** that represents the amount of horizontal space between the invisible gridlines that Microsoft Word uses when you draw, move, and resize AutoShapes or East Asian characters in the specified document. Read/write.


## Syntax

 _expression_ . **GridDistanceHorizontal**

 _expression_ A variable that represents a **[Document](8d83487a-2345-a036-a916-971c9db5b7fb.md)** object.


## Example

This example sets the horizontal and vertical distance between gridlines and then enables the Snap objects to grid feature for the current document.


```vb
With ActiveDocument 
 .GridDistanceHorizontal = 9 
 .GridDistanceVertical = 9 
 .SnapToGrid = True 
End With
```


## See also


#### Concepts


[Document Object](8d83487a-2345-a036-a916-971c9db5b7fb.md)
#### Other resources


[Document Object Members](fc9ab457-0888-f917-3d52-387168ac23b9.md)
