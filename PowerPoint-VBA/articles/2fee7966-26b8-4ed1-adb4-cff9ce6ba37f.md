
# SlideRange.SlideNumber Property (PowerPoint)

Returns the slide number. Read-only.


## Syntax

 _expression_. **SlideNumber**

 _expression_ A variable that represents a **SlideRange** object.


### Return Value

Integer


## Remarks

The  **SlideNumber** property of a **Slide** object is the actual number that appears in the lower-right corner of the slide when you display slide numbers. This number is determined by the number of the slide within the presentation (the **[SlideIndex](d913a70f-eb31-73b0-43bc-1021b3195a7e.md)** property value) and the starting slide number for the presentation (the **[FirstSlideNumber](277f613b-8c3a-d8bb-593c-a66ca41b4fa0.md)** property value). The slide number is always equal to the starting slide number + the slide index number - 1.


## Example

This example shows how changing the first slide number affects the slide number of a specific slide.


```
With Application.ActivePresentation

    .PageSetup.FirstSlideNumber = 1   'starts slide numbering at 1

    MsgBox .Slides(2).SlideNumber     'returns 2



    .PageSetup.FirstSlideNumber = 10 'starts slide numbering at 10

    MsgBox .Slides(2).SlideNumber     'returns 11

End With
```


## See also


#### Concepts


[SlideRange Object](440ab59d-744a-209f-bf28-d0acd3a21e1a.md)
#### Other resources


[SlideRange Object Members](f819c56d-96d5-836d-0d1f-49e505696f34.md)
