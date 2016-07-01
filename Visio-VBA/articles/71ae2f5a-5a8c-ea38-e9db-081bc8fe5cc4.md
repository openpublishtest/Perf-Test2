
# Application.LanguageHelp Property (Visio)

Represents the language ID of the Help in the version of the Microsoft Visio instance represented by the parent object. Read-only.


## Syntax

 _expression_ . **LanguageHelp**

 _expression_ A variable that represents an **Application** object.


### Return Value

Long


## Remarks

The  **LanguageHelp** property returns the language ID of the Help recorded in the object's VERSIONINFO resource. The IDs returned are the standard IDs used by Microsoft Windows to encode different language versions. For example, the **LanguageHelp** property returns &amp;H0409 for the U.S. English version of Visio. For details, search for "VERSIONINFO" in the Microsoft Platform SDK on MSDN.

