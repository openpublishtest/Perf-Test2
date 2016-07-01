
# Presentation.PasswordEncryptionKeyLength Property (PowerPoint)

Returns the key length of the algorithm Microsoft PowerPoint uses when it encrypts documents with passwords. Read-only.


## Syntax

 _expression_. **PasswordEncryptionKeyLength**

 _expression_ A variable that represents a **Presentation** object.


### Return Value

Long


## Remarks

Use the  **[SetPasswordEncryptionOptions](03c07952-784b-eba6-af71-57d3d1414f81.md)** method to specify the algorithm PowerPoint uses for encrypting documents with passwords.


## Example

This example sets the password encryption options if the password encryption key length is less than 40.


```
Sub PasswordSettings() 
    With ActivePresentation 
        If .PasswordEncryptionKeyLength < 40 Then 
            .SetPasswordEncryptionOptions  


PasswordEncryptionProvider:="Microsoft RSA SChannel Cryptographic Provider", _ 
                PasswordEncryptionAlgorithm:="RC4", _ 
                PasswordEncryptionKeyLength:=56, _ 
                PasswordEncryptionFileProperties:=True 
        End If 
    End With 
End Sub


```


## See also


#### Concepts


[Presentation Object](ec75cf52-69f8-d35b-0a26-4a8da8a9683f.md)
#### Other resources


[Presentation Object Members](b3538c7e-5fd9-d34d-ab5c-0105dbd516d0.md)
