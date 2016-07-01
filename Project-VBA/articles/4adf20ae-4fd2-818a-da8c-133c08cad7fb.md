
# Application.SelectBeginning Method (Project)

Selects the first cell in the active table or view.


## Syntax

 _expression_. **SelectBeginning**( ** _Extend_** )

 _expression_ A variable that represents an **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Extend_|Optional|**Boolean**|**True** if the current selection is extended to the first cell. If the active view is the Network Diagram or Resource Graph, Extend is ignored. The default value is **False**.|

### Return Value

 **Boolean**


## Remarks

In the Resource Graph,  **SelectBeginning** selects the resource with the lowest identification number. In the Network Diagram, **SelectBeginning** selects the box closest to the upper-left corner of the view.


## Example

The following example selects the "Name" field of row 4 as the beginning field in the Gantt Chart.


```
Sub Select_Beginning() 
 
 ViewApply Name:="&amp;Gantt Chart" 
 SelectTaskField Row:=4, Column:="Name", RowRelative:=False 
 
 SelectBeginning Extend:=True 
End Sub
```

