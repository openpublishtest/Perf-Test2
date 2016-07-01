
# Application.AlignTableCellBottom Method (Project)
Aligns text at the bottom of the cell, for selected cells in a report table.

## Syntax

 _expression_. **AlignTableCellBottom**

 _expression_ A variable that represents an **Application** object.


### Return value

 **Boolean**


## Example

In the following example, the  **AlignTableCells** macro aligns the text for all tables in the specified report.


```
Sub TestAlignReportTables()
    Dim reportName As String
    Dim alignment As String   ' The value can be "top", "center", or "bottom".
    
    reportName = "Align Table Cells Report"
    alignment = "top"
    
    AlignTableCells reportName, alignment
End Sub

' Align the text for all tables in a specified report.
Sub AlignTableCells(reportName As String, alignment As String)
    Dim theReport As Report
    Dim shp As Shape
    
    Set theReport = ActiveProject.Reports(reportName)
    
    ' Activate the report. If the report is already active,
    ' ignore the run-time error 1004 from the Apply method.
    On Error Resume Next
    theReport.Apply
    On Error GoTo 0
    
    For Each shp In theReport.Shapes
        Debug.Print "Shape: " &amp; shp.Type &amp; ", " &amp; shp.Name
        
        If shp.HasTable Then
            shp.Select
            
            Select Case alignment
                Case "top"
                    AlignTableCellTop
                Case "center"
                    AlignTableCellVerticalCenter
                Case "bottom"
                    AlignTableCellBottom
                Case Else
                    Debug.Print "AlignTableCells error: " &amp; vbCrLf _
                        &amp; "alignment must be top, center, or bottom."
                End Select
        End If
    Next shp
End Sub
```


## See also


#### Concepts


[Application Object](8eb91712-7784-a102-38c0-19bb056c27e9.md)
#### Other resources


[Report Object](38ef993e-e5cd-b451-06aa-41eb0e93450e.md)
[AlignTableCellTop Method](51eca157-64c4-f114-243e-895d97adf45a.md)
[AlignTableCellVerticalCenter Method](c790d8f7-e792-0718-3166-312640ff3f73.md)