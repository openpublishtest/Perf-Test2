
# Shapes.Value Property (Project)
Gets an individual  **Shape** object in the **Shapes** collection. Read-only **Shape**.

## Syntax

 _expression_. **Value**

 _expression_ A variable that represents a **Shapes** object.


### Parameters



|**Name**|**Required/Optional**|**Data type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Index_|Required|**Variant**|Can be a  **String** value for the name of the shape or a **Long** value for the ordinal index number of the shape.|

## Remarks

 **Value** is the default property for the **Shapes** object. For example, create a report namedTable Tests that contains a table. The following statement in the **Immediate** window of the VBE prints the name of the table.


```
? ActiveProject.Reports("Table Tests").Shapes.Value(1).Name
```

If you leave off the  **Shapes** property, the following statement is effectively the same as the previous statement.




```
? ActiveProject.Reports("Table Tests").Shapes(1).Name
```

 **Shapes.Item** acts like **Shapes.Value**, except  **Item** is a method:




```
? ActiveProject.Reports("Table Tests").Shapes.Item(1).Name
```


## Property value

 **SHAPE**


## See also


#### Other resources


[Shapes Object](6e42040c-dd5a-de4c-afa8-f9e33d1e5054.md)
[Item Method](43fba4f4-f3d3-20a0-2c77-15e31dcdcbf5.md)