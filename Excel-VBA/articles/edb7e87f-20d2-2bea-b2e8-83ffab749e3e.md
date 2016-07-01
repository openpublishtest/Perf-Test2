
# Style.IncludePatterns Property (Excel)

 **True** if the style includes the **Color** , **ColorIndex** , **InvertIfNegative** , **Pattern** , **PatternColor** , and **PatternColorIndex** interior properties. Read/write **Boolean** .


## Syntax

 _expression_ . **IncludePatterns**

 _expression_ A variable that represents a **Style** object.


## Example

This example sets the style attached to cell A1 on Sheet1 to include pattern format.


```vb
Worksheets("Sheet1").Range("A1").Style.IncludePatterns = True
```


## See also


#### Concepts


[Style Object](3c1e9184-0075-5f46-9a1a-0b61d874d1f8.md)
#### Other resources


[Style Object Members](78f477c9-4033-e7c5-fc3d-7ba025392d31.md)
