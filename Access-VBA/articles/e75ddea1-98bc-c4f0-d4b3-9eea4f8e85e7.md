
# Label.BorderThemeColorIndex Property (Access)

Gets or sets a value that represents a color in the applied color theme associated with the  **BorderColor** property of the specified object. Read/write **Long**.


## Syntax

 _expression_. **BorderThemeColorIndex**

 _expression_ A variable that represents a **Label** object.


## Remarks

The  **BorderThemeColorIndex** property contains one of the index values listed in the following table.



|**Index Value**|**Description**|
|:-----|:-----|
|0|Text 1|
|1|Background 1|
|2|Text 2|
|3|Background 2|
|4|Accent 1|
|5|Accent 2|
|6|Accent 3|
|7|Accent 4|
|8|Accent 5|
|9|Accent 6|
|10|Hyperlink|
|11|Followed Hyperlink|
If no theme is applied, the  **BorderThemeColorIndex** property contains -1.

This property is not surfaced in the property sheet.


## Example

The following code example sets the Border Color to the Text 2 color by setting the  **BorderThemeColorIndex** property.


```
Me.ctl.BorderThemeColorIndex=2
```


## See also


#### Concepts


[Label Object](3d83d916-85d7-b2eb-c9f6-f9a6ff0c9ec7.md)
#### Other resources


[Label Object Members](a47442ed-c770-49a4-3bd1-76e3e05bddca.md)