
# Application.SelectResourceColumn Method (Project)

Selects a column containing resource information.


## Syntax

 _expression_. **SelectResourceColumn**( ** _Column_**, ** _Additional_**, ** _Extend_**, ** _Add_** )

 _expression_ A variable that represents an **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Column_|Optional|**String**|The field name of the column to select. The default is the column containing the active cell.|
| _Additional_|Optional|**Integer**|The number of additional columns to select to the right of  **Column**. If **Extend** is **True**, **Additional** is ignored. The default value is 0.|
| _Extend_|Optional|**Boolean**|**True** if all columns between the current selection and **Column** are selected. The default value is **False**.|
| _Add_|Optional|**Boolean**|**True** if the current column is included in the selection. The default value is **False**.|

### Return Value

 **Boolean**


## Remarks

The  **SelectResourceColumn** method is only available when the Resource Sheet or Resource Usage view is the active view.


## Example

The following example selects the  **Indicators** column and the next two columns.


```
Sub Select_ResourceColumn() 
 
 'Activate Resource Sheet 
 ViewApply Name:="&amp;Resource Sheet" 
 SelectResourceColumn Column:="Indicators", Additional:=2 
End Sub
```

