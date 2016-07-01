
# TextRange.BoundTop Property (PowerPoint)

Returns the distance (in points) from the top of the of the text bounding box for the specified text frame to the top of the slide. Read-only.


## Syntax

 _expression_. **BoundTop**

 _expression_ A variable that represents a **TextRange** object.


### Return Value

Single


## Example

This example adds a rounded rectangle to slide one in the active presentation. The rectangle has the same dimensions as the text bounding box for shape one.


```
With Application.ActivePresentation.Slides(1).Shapes

    Set tr = .Item(1).TextFrame.TextRange

    Set roundRect = .AddShape(msoShapeRoundedRectangle, _

        tr.BoundLeft, tr.BoundTop, tr.BoundWidth, tr.BoundHeight)

End With

With roundRect.Fill

    .ForeColor.RGB = RGB(255, 0, 128)

    .Transparency = 0.75

End With
```


## See also


#### Concepts


[TextRange Object](7c234107-c423-7ec9-e8bd-a82cc3b345de.md)
#### Other resources


[TextRange Object Members](cb8dc5ff-34de-3d04-1d56-ed387daaf6b9.md)
