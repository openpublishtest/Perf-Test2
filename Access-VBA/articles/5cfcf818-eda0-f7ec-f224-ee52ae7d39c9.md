
# Form.DatasheetFontHeight Property (Access)

You can use the  **DatasheetFontHeight** property to specify the font point size used to display and print field names and data in Datasheet view. Read/write **Integer**.


## Syntax

 _expression_. **DatasheetFontHeight**

 _expression_ A variable that represents a **Form** object.


## Remarks

This property is only available within a Microsoft Access database.

For the  **DatasheetFontHeight** property, the font size you specify must be valid for the font specified by the **DatasheetFontName** property. For example, MS Sans Serif is available only in sizes 8, 10, 12, 14, 18, and 24 points.

The following table contains the properties that don't exist in the DAO  **Properties** collection of until you set them by using the **Formatting (Datasheet)** toolbar or you can add them in an Access database (.mdb) by using the **CreateProperty** method and append it to the **DAO Properties** collection.


|||
|:-----|:-----|
|**[DatasheetFontItalic](32fe51fa-ee36-2fc3-bb72-e61a4b43c19c.md)** *|**[DatasheetForeColor](9756ff09-67bf-edb9-d4b5-d414ec7c1e2a.md)** *|
|**[DatasheetFontHeight](5cfcf818-eda0-f7ec-f224-ee52ae7d39c9.md)** *|**[DatasheetBackColor](69734522-e570-86a5-f971-ce26ee4f88c3.md)**|
|**[DatasheetFontName](e6b963ca-7162-912e-e63d-1437904ec8f1.md)** *|**[DatasheetGridlinesColor](92d07c1c-fc47-0049-7da3-a34ee56fbc83.md)**|
|**[DatasheetFontUnderline](a232a1a8-b537-4935-bd64-138548241c7c.md)** *|**[DatasheetGridlinesBehavior](692268ab-69f2-4891-e460-f091b43af962.md)**|
|**[DatasheetFontWeight](6dd2c6d3-1f27-8b86-abf5-f5581fbe7d23.md)** *|**[DatasheetCellsEffect](3820b218-37b0-d5b5-bae2-8a179cc9b87a.md)**|

 **Note**  When you add or set any property listed with an asterisk, Microsoft Access automatically adds all the properties listed with an asterisk to the  **Properties** collection of the database.


## Example

The following example sets the font to MS Serif, the font size to 10 points, and the font weight to medium (500) in Datasheet view of the Products table.


```
Sub SetDatasheetFont 
 
 Dim dbs As Object, objProducts As Object 
 Set dbs = CurrentDb 
 Const DB_Text As Long = 10 
 Const DB_Integer As Long = 3 
 Set objProducts = dbs!Products 
 
 SetTableProperty objProducts, "DatasheetFontName", DB_Text, "MS Serif" 
 SetTableProperty objProducts, "DatasheetFontHeight", DB_Integer, 10 
 SetTableProperty objProducts, "DatasheetFontWeight", DB_Integer, 500 
 
End Sub 
 
 
 
Sub SetTableProperty(objTableObj As Object, strPropertyName As String, _ 
 intPropertyType As Integer, varPropertyValue As Variant) 
 ' Set Microsoft Access-defined table property without causing 
 ' nonrecoverable run-time error. 
 Const conErrPropertyNotFound = 3270 
 Dim prpProperty As Variant 
 On Error Resume Next ' Don't trap errors. 
 objTableObj.Properties(strPropertyName) = varPropertyValue 
 If Err <> 0 Then ' Error occurred when value set. 
 If Err <> conErrPropertyNotFound Then 
 On Error GoTo 0 
 MsgBox "Couldn't set property '" &amp; strPropertyName _ 
 &amp; "' on table '" &amp; objTableObj.Name &amp; "'", 48, "SetTableProperty" 
 Else 
 On Error GoTo 0 
 Set prpProperty = objTableObj.CreateProperty(strPropertyName, _ 
 intPropertyType, varPropertyValue) 
 objTableObj.Properties.Append prpProperty 
 End If 
 End If 
 objTableObj.Properties.Refresh 
End Sub
```

The next example makes the same changes as the preceding example in Datasheet view of the open Products form.




```
Forms!Products.DatasheetFontName = "MS Serif" 
Forms!Products.DatasheetFontHeight = 10 
Forms!Products.DatasheetFontWeight = 500
```


## See also


#### Concepts


[Form Object](72ef9219-142b-b690-b696-3eba9a5d4522.md)
#### Other resources


[Form Object Members](e1976b58-28ca-8f76-cdf3-6732cb06ce6c.md)