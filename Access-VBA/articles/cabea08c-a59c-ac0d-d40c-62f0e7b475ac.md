
# NavigationControl.BackTint Property (Access)

Gets or sets the tint that is applied to the theme color in the  **BackColor** property of the specified object. Read/write **Single**.


## Syntax

 _expression_. **BackTint**

 _expression_ A variable that represents a **NavigationControl** object.


## Remarks

The  **BackTint** property contains a numeric expression that can be used to lighten the theme color in the **BackColor** property. The default value of the **BackTint** property is 100, which is neutral, and does not change the theme color. To lighten the color, first determine the percentage by which to lighten from 1 to 100, then subtract that value as a whole number from 100 and use the remainder. For example, to lighten the theme color tint by 75%, subtract 75 from 100 and use the remainder, which is 25.

This property is not surfaced in the property sheet.


## Example

The following code example lightens the  **BackColor** by 75%.


```
Me.ctl.BackTint=25
```


## See also


#### Concepts


[NavigationControl Object](ab08e35c-e5e4-444c-d169-1092d282ed15.md)
#### Other resources


[NavigationControl Object Members](c972327e-9b46-f9fb-d69d-104d1d130ee4.md)