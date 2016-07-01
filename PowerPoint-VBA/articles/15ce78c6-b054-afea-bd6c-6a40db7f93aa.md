
# Axis.MinorUnitScale Property (PowerPoint)

Returns or sets the minor unit scale value for the category axis when the  **[CategoryType](bbcb485d-9464-33c8-ca9b-e3463bc9e884.md)** property is set to **xlTimeScale**. Read/write **[XlTimeUnit](7da25d66-7339-9cb2-13da-81dda86a55b4.md)**.


## Syntax

 _expression_. **MinorUnitScale**

 _expression_ A variable that represents an **[Axis](38d5e006-ac32-7bdb-f9f0-e8a858dcbf49.md)** object.


## Remarks

 **MinorUnitScale** can be one of the following **XlTimeUnit** constants:


-  **xlMonths**
    
-  **xlDays**
    
-  **xlYears**
    

## Example




 **Note**  Although the following code applies to Microsoft Word, you can readily modify it to apply to PowerPoint.

The following example sets the category axis to use a time scale and sets the major and minor units.




```
With ActiveDocument.InlineShapes(1)

    If .HasChart Then

        With .Chart.Axes(xlCategory)

            .CategoryType = xlTimeScale

            .MajorUnit = 5

            .MajorUnitScale = xlDays

            .MinorUnit = 1

            .MinorUnitScale = xlDays

        End With

    End If

End With
```


## See also


#### Concepts


[Axis Object](38d5e006-ac32-7bdb-f9f0-e8a858dcbf49.md)
#### Other resources


[Axis Object Members](6c4c7cca-d62e-a7c0-b724-30d1be8a44c9.md)
