
# ObjectFrame.BorderTint Property (Access)

Gets or sets the tint that is applied to the theme color in the  **BorderColor** property of the specified object. Read/write **Single**.


## Syntax

 _expression_. **BorderTint**

 _expression_ A variable that represents an **ObjectFrame** object.


## Remarks

The  **BorderTint** property contains a numeric expression that can be used to lighten the theme color in the **BorderColor** property. The default value of the **BorderTint** property is 100, which is neutral, and does not change the theme color. To lighten the color, first determine the percentage by which to lighten from 1 to 100, then subtract that value as a whole number from 100 and use the remainder. For example, to lighten the theme color by 75%, subtract 75 from 100 and use the remainder, which is 25.

This property is not surfaced in the property sheet.


## Example

The following code example lightens  **BorderColor** by 75%.


```
Me.ctl.BorderTint=25
```


## See also


#### Concepts


[ObjectFrame Object](0eb85477-58d7-249a-2bf7-f2f3960a45a9.md)
#### Other resources


[ObjectFrame Object Members](65229083-68ec-b870-50f4-a6c329259a39.md)