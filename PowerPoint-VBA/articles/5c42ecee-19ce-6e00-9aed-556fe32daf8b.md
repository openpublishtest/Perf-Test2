
# Presentations.Application Property (PowerPoint)

Returns an  **[Application](978c2b99-4271-b953-4283-73b5f3d96f41.md)** object that represents the creator of the specified object.


## Syntax

 _expression_. **Application**

 _expression_ A variable that represents a **Presentations** object.


### Return Value

Application


## Example

In this example, a  **[Presentation](ec75cf52-69f8-d35b-0a26-4a8da8a9683f.md)** object is passed to the procedure. The procedure adds a slide to the presentation and then saves the presentation in the folder where Microsoft PowerPoint is running.


```
Sub AddAndSave(pptPres As Presentation)

    pptPres.Slides.Add 1, 1

    pptPres.SaveAs pptPres.Application.Path &amp; "\Added Slide"

End Sub
```

This example displays the name of the application that created each linked OLE object on slide one in the active presentation.




```
For Each shpOle In ActivePresentation.Slides(1).Shapes

    If shpOle.Type = msoLinkedOLEObject Then

        MsgBox shpOle.OLEFormat.Application.Name

    End If

Next
```


## See also


#### Concepts


[Presentations Object](0b952edc-8628-71ef-e854-3bcefbb3bc61.md)
#### Other resources


[Presentations Object Members](b113aad2-7236-40a6-8c21-8217feff0d6b.md)
