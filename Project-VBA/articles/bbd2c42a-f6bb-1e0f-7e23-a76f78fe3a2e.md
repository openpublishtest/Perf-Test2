
# Task.ActualOvertimeWork Property (Project)

Gets the actual overtime work (in minutes) for a task. Read-only  **Variant**.


## Syntax

 _expression_. **ActualOvertimeWork**

 _expression_ A variable that represents a **Task** object.


## Example

The following example shows the cost of overtime by calculating the total cost of tasks with overtime work, as well as breaking down the individual costs per task.


```
Sub PriceOfOvertime() 
 Dim T As Task 
 Dim Price As Variant 
 Dim Breakdown As String 
 
 For Each T In ActiveProject.Tasks 
 If Not (T Is Nothing) Then 
 If T.ActualOvertimeWork <> 0 Then 
 Price = Price + T.ActualOvertimeCost 
 Breakdown = Breakdown &amp; T.Name &amp; ": " &amp; _ 
 ActiveProject.CurrencySymbol &amp; _ 
 T.ActualOvertimeCost &amp; vbCrLf 
 End If 
 End If 
 Next T 
 
 If Breakdown <> "" Then 
 MsgBox Breakdown &amp; vbCrLf &amp; "Total: " &amp; _ 
 ActiveProject.CurrencySymbol &amp; Price 
 End If 
 
End Sub
```

