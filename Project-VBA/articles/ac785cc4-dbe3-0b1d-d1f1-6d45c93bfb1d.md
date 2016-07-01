
# GroupCriteria2 Object (Project)

Contains a collection of  **[GroupCriterion2](06047a9d-a9db-43e0-e759-e24560da7128.md)** objects, where the group hierarchy can be maintained and cell color can be a hexadecimal value.


## Example

 **Using the GroupCriterion2 Object**

Use  **GroupCriteria2(** _Index_ **)**, where _Index_ is the criterion index, to return a single **GroupCriterion2** object. The following example sets the cell color for the first criterion in the Standard Rate resource group to blue.




```
ActiveProject.ResourceGroups2("Standard Rate").GroupCriteria2(1).CellColor = &amp;HFF0000
```

 **Using the GroupCriteria2 Collection**

Use the  **[GroupCriteria](0c6d6412-cd7b-7b12-1740-7cd5cd38aaf1.md)** property to return a **GroupCriteria2** collection. The following example displays a list of the fields used as criteria in the specified task group and shows whether they are sorted in ascending or descending order.




```
Dim GC2 As GroupCriterion2  
Dim Fields As String  
  
For Each GC2 In ActiveProject.TaskGroups2("Priority Keeping Outline Structure").GroupCriteria  
    If GC2.Ascending = True Then  
       Fields = Fields &amp; GC2.Index &amp; ". " &amp; GC2.FieldName &amp; " is sorted in ascending order." _
           &amp; vbCrLf  
    Else  
        Fields = Fields &amp; GC2.Index &amp; ". " &amp; GC2.FieldName &amp; " is sorted in descending order." _
           &amp; vbCrLf  
    End If  
Next GC2  

MsgBox Fields
```

Use the  **[AddEx](8474aa63-bf63-be29-86ef-177d8105e105.md)** method to add a **GroupCriterion2** object to the **GroupCriteria2** collection, where **CellColor** can be a hexadecimal value. The following example adds another criterion to the specified resource group, grouping resources in ascending order as determined by the percentage of their work (in 25-percent increments) that is complete.




```
ActiveProject.ResourceGroups2("Response Pending").GroupCriteria2.AddEx "% Work Complete", True, _  
    CellColor:=&amp;H0101FF, GroupOn:=pjGroupOnPct1_25
```


## See also


#### Concepts


[Project Object Model](900b167b-88ec-ea88-15b7-27bb90c22ac6.md)
#### Other resources


[GroupCriteria2 Object Members](b52e84f3-4332-9c5a-cd2c-c4b57cfc40ea.md)