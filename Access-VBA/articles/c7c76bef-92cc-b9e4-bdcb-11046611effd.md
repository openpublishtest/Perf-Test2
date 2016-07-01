
# SubForm.Report Property (Access)

You can use the  **Report** property to refer to a report or to refer to the report associated with a subreport control. Read-only **Report**.


## Syntax

 _expression_. **Report**

 _expression_ A variable that represents a **SubForm** object.


## Remarks

This property is typically used to refer to the report contained in a subreport control.


 **Note**  When you use the  **[Reports](37c5f55e-3c3a-6140-d305-7e8118d9d2b1.md)** collection, you must specify the name of the report.


## Example

The following example uses the  **Report** property to refer to a control on a subreport.


```
Dim curTotalSales As Currency 
 
curTotalSales = Reports!Sales!Employees.Report!TotalSales
```


## See also


#### Concepts


[SubForm Object](60f961fa-dcf4-e1d1-8c50-9e88963f9dec.md)
#### Other resources


[SubForm Object Members](328e74d8-0418-968f-faca-3e1b34139f48.md)