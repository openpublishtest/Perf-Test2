
# Report.ScaleWidth Property (Access)

You can use the  **ScaleWidth** property to specify the number of units for the horizontal measurement of the page when the **[Circle](4f5d24e2-75bf-3586-7e0d-0902adee61a6.md)**, **[Line](9e640e37-c055-3dc3-b70e-0805cdc13561.md)**, **[Pset](951a262b-b17b-9b95-b5f2-922d4aff9ce9.md)**, or **[Print](6f8523cc-7b17-ec27-e2c9-a7ae3d5a8c3f.md)** method is used while a report is printed or previewed, or its output is saved to a file. Read/write **Single**.


## Syntax

 _expression_. **ScaleWidth**

 _expression_ A variable that represents a **Report** object.


## Remarks

The default setting is the internal width of a report page in twips.

You can set the  **ScaleWidth** property by using a macro or a[Visual Basic](3fa3677b-a779-3bc7-0f0f-827c252b3292.md)event procedure specified by a section's **OnPrint** property setting.

You can use the  **ScaleWidth** property to create a custom coordinate scale for drawing or printing. For example, the statement `ScaleWidth = 100` defines the internal width of the section as 100 units, or one horizontal unit as one one-hundredth of the width.

Use the  **[ScaleMode](e3955e48-80bb-989e-2992-cd5a541b468b.md)** property to define a scale based on a standard unit of measurement, such as points, pixels, characters, inches, millimeters, or centimeters.

Setting the  **ScaleWidth** property to a positive value makes coordinates increase in value from left to right. Setting it to a negative value makes coordinates increase in value from right to left.

By using these properties and the related  **ScaleLeft** and **ScaleTop** properties, you can set up a custom coordinate system with both positive and negative coordinates. All four of these Scale properties interact with the **ScaleMode** property in the following ways:


- Setting any other Scale property to any value automatically sets the  **ScaleMode** property to 0.
    
- Setting the  **ScaleMode** property to a number greater than 0 changes the **ScaleHeight** and **ScaleWidth** properties to the new unit of measurement and sets the **ScaleLeft** and **ScaleTop** properties to 0. Also, the **CurrentX** and **CurrentY** property settings change to reflect the new coordinates of the current point.
    
You can also use the  **Scale** method to set the **ScaleHeight**, **ScaleWidth**, **ScaleLeft**, and **ScaleTop** properties in one statement.


 **Note**  The  **ScaleWidth** properties isn't the same as the **Width** property.


## Example

The following example uses the  **Print** method to display text on a report named Report1. It uses the **TextWidth** and **TextHeight** methods to center the text vertically and horizontally.


```
Private Sub Detail_Format(Cancel As Integer, _ 
 FormatCount As Integer) 
 Dim rpt as Report 
 Dim strMessage As String 
 Dim intHorSize As Integer, intVerSize As Integer 
 
 Set rpt = Me 
 strMessage = "DisplayMessage" 
 With rpt 
 'Set scale to pixels, and set FontName and 
 'FontSize properties. 
 .ScaleMode = 3 
 .FontName = "Courier" 
 .FontSize = 24 
 End With 
 ' Horizontal width. 
 intHorSize = Rpt.TextWidth(strMessage) 
 ' Vertical height. 
 intVerSize = Rpt.TextHeight(strMessage) 
 ' Calculate location of text to be displayed. 
 Rpt.CurrentX = (Rpt.ScaleWidth/2) - (intHorSize/2) 
 Rpt.CurrentY = (Rpt.ScaleHeight/2) - (intVerSize/2) 
 ' Print text on Report object. 
 Rpt.Print strMessage 
End Sub
```


## See also


#### Concepts


[Report Object](6f77c1b4-a9ce-7caa-204c-fe0755c6f9df.md)
#### Other resources


[Report Object Members](73370a33-1ca0-da4d-9e36-88011bc2b93e.md)