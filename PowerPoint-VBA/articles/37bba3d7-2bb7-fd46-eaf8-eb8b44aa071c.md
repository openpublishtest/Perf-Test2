
# Point.SecondaryPlot Property (PowerPoint)

 **True** if the point is in the secondary section of either a pie-of-pie chart or a bar-of-pie chart. Read/write **Boolean**.


## Syntax

 _expression_. **SecondaryPlot**

 _expression_ A variable that represents a **[Point](e0137fdd-5632-88d7-a6c0-57a76717e736.md)** object.


## Remarks

This property applies only to points on pie-of-pie charts or bar-of-pie charts. 


## Example




 **Note**  Although the following code applies to Microsoft Word, you can readily modify it to apply to PowerPoint.

The following example moves point four to the secondary section of the chart. You must run this example on either a pie-of-pie chart or a bar-of-pie chart. 




```
With ActiveDocument.InlineShapes(1)

    If .HasChart Then

        With .Chart.SeriesCollection(1)

            .Points(4).SecondaryPlot = True

        End With

    End If

End With
```


## See also


#### Concepts


[Point Object](e0137fdd-5632-88d7-a6c0-57a76717e736.md)
#### Other resources


[Point Object Members](ddf0303f-d97f-91fd-12b5-e569a7899ebd.md)
