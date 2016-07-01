
# Editors Object (Word)

A collection of  **Editor** objects that represents a collection of users or groups of users who have been given specific permissions to edit portions of a document.


## Remarks

Use the  **Add** method to give a specified user or group permission to modify a range or selection within a document. The following example gives the current user editing permission to modify the active selection.


```vb
Dim objEditor As Editor 
 
Set objEditor = Selection.Editors.Add(wdEditorCurrent)
```


## See also


#### Other resources


[Editors Object Members](dcb26f83-bbff-8d3a-2493-f7d87ce40d21.md)
[Word Object Model Reference](http://msdn.microsoft.com/library/be452561-b436-bb9b-6f94-3faa9a74a6fd%28Office.15%29.aspx)
