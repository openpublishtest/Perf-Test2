
# ContactItem.CompanyLastFirstNoSpace Property (Outlook)

Returns a  **String** representing the company name for the contact followed by the concatenated last name, first name, and middle name with no space between the last and first names. Read-only.


## Syntax

 _expression_ . **CompanyLastFirstNoSpace**

 _expression_ A variable that represents a **ContactItem** object.


## Remarks

This property is parsed from the  **[CompanyName](076cd6f7-7faa-ab1c-254c-3307c40520ee.md)** , **[LastName](430682f6-a230-887b-404b-a71989121fa2.md)** , **[FirstName](403b5e5a-037b-cf21-efc2-2bd2a80c3789.md)** , and **[MiddleName](07e0c9b1-1093-2f8a-3b89-ba8570b2bdf5.md)** properties. The **LastName** , **FirstName** , and **MiddleName** properties are themselves parsed from the **[FullName](3036dc57-31fb-45ad-f51e-49336206581d.md)** property. The value of this property is only filled when its associated property ( **FirstName** , **LastName** , **MiddleName** , **CompanyName** , and **Suffix** ) contain Asian (DBCS) characters. If the corresponding field does not contain Asian characters, the property will be empty.


## See also


#### Concepts


[ContactItem Object](8e32093c-a678-f1fd-3f35-c2d8994d166f.md)
#### Other resources


[ContactItem Object Members](a8b13369-4c87-02aa-e62a-1f3067e559fa.md)
