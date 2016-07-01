
# Options.SaveAutoRecoverInfoInterval Property (Publisher)

Returns or sets a  **Long** that represents the time interval in minutes for automatically saving a publication for recovery if the application is unexpectedly shut down. Read/write.


## Syntax

 _expression_. **SaveAutoRecoverInfoInterval**

 _expression_A variable that represents a  **Options** object.


### Return Value

Long


## Example

This example enables the global auto recovery option and sets the save interval to every five minutes.


```vb
Sub SetAutoRecoverInfo() 
 With Options 
 .SaveAutoRecoverInfo = True 
 .SaveAutoRecoverInfoInterval = 5 
 End With 
End Sub
```

