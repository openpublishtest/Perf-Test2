
# Options.AutoFormatApplyFirstIndents Property (Word)

 **True** if Microsoft Word replaces a space entered at the beginning of a paragraph with a first-line indent when Word formats a document or range automatically. Read/write **Boolean** .


## Syntax

 _expression_ . **AutoFormatApplyFirstIndents**

 _expression_ An expression that returns an **[Options](873b7b99-3fe1-fd89-9ece-a9355cb827dc.md)** object.


## Example

This example sets Microsoft Word to replace a space entered at the beginning of a paragraph with a first-line indent and automatically formats the selected range.


```vb
Options.AutoFormatApplyFirstIndents = True 
Selection.Range.AutoFormat
```


## See also


#### Concepts


[Options Object](873b7b99-3fe1-fd89-9ece-a9355cb827dc.md)
#### Other resources


[Options Object Members](76cd9dfe-6bbb-4c3d-0bfc-79a62bedd15e.md)
