
# Workspace.CreateDatabase Method (DAO)

 **Last modified:** March 09, 2015

 _ **Applies to:** Access 2013 | Access 2016_

 **In this article**
[Syntax](#sectionSection0)
[Remarks](#sectionSection1)
[Example](#sectionSection2)


Creates a new  **[Database](6cf2ddf8-3957-a15e-5eeb-85f81c1e415e.md)** object, saves the database to disk, and returns an opened **Database** object (Microsoft Access workspaces only).

## Syntax
<a name="sectionSection0"> </a>

 _expression_. **CreateDatabase**( ** _Name_**, ** _Connect_**, ** _Option_** )

 _expression_ A variable that represents a **Workspace** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _Name_|Required|**String**|A String up to 255 characters long that is the name of the database file that you're creating. It can be the full path and file name. If your network supports it, you can also specify a network path, such as "\\server1\share1\dir1\db1". You can only create Microsoft Access database files with this method.|
| _Connect_|Required|**String**|
<ul xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:mtps="http://msdn2.microsoft.com/mtps" xmlns:mshelp="http://msdn.microsoft.com/mshelp" xmlns:ddue="http://ddue.schemas.microsoft.com/authoring/2003/5" xmlns:msxsl="urn:schemas-microsoft-com:xslt"><li><p>A string expression that specifies a collating order for creating the database, as specified in Settings. You must supply this argument or an error occurs.</p></li><li><p>You can also create a password for the new <b>Database</b>  object by concatenating the password string (starting with <span class="code">";pwd="</span>) with a constant in the <i>locale</i>  argument, like this:</p></li><li><p><span class="code">dbLangSpanish &amp; ";pwd=NewPassword"</span></p></li><li><p>If you want to use the default <i>locale</i> , but specify a password, simply enter a password string for the <i>locale</i>  argument:</p></li><li><p><span class="code">";pwd=NewPassword"</span></p></li><li><p>Use strong passwords that combine upper- and lowercase letters, numbers, and symbols. Weak passwords don't mix these elements. Strong password: Y6dh!et5. Weak password: House27. Use a strong password that you can remember so that you don't have to write it down.</p></li></ul>|
| _Option_|Optional|**Variant**|A constant or combination of constants that indicates one or more options, as specified in Settings. You can combine options by summing the corresponding constants.|

## Remarks
<a name="sectionSection1"> </a>

You can use one of the following constants for the locale argument to specify the [CollatingOrder](7f6c35bf-e5f9-8423-608e-bc072ca09141.md) property of text for string comparisons.



|**Constant**|**Collating order**|
|:-----|:-----|
|**dbLangGeneral**|English, German, French, Portuguese, Italian, and Modern Spanish|
|**dbLangArabic**|Arabic|
|**dbLangChineseSimplified**|Simplified Chinese|
|**dbLangChineseTraditional**|Traditional Chinese|
|**dbLangCyrillic**|Russian|
|**dbLangCzech**|Czech|
|**dbLangDutch**|Dutch|
|**dbLangGreek**|Greek|
|**dbLangHebrew**|Hebrew|
|**dbLangHungarian**|Hungarian|
|**dbLangIcelandic**|Icelandic|
|**dbLangJapanese**|Japanese|
|**dbLangKorean**|Korean|
|**dbLangNordic**|Nordic languages (Microsoft Jet database engine version 1.0 only)|
|**dbLangNorwDan**|Norwegian and Danish|
|**dbLangPolish**|Polish|
|**dbLangSlovenian**|Slovenian|
|**dbLangSpanish**|Traditional Spanish|
|**dbLangSwedFin**|Swedish and Finnish|
|**dbLangThai**|Thai|
|**dbLangTurkish**|Turkish|
You can use one or more of the following constants in the options argument to specify which version the data format should have and whether or not to encrypt the database.



|**Constant**|**Description**|
|:-----|:-----|
|**dbEncrypt**|Creates an encrypted database.|
|**dbVersion10**|Creates a database that uses the Microsoft Jet database engine version 1.0 file format.|
|**dbVersion11**|Creates a database that uses the Microsoft Jet database engine version 1.1 file format.|
|**dbVersion20**|Creates a database that uses the Microsoft Jet database engine version 2.0 file format.|
|**dbVersion30**|Creates a database that uses the Microsoft Jet database engine version 3.0 file format (compatible with version 3.5).|
|**dbVersion40**|Creates a database that uses the Microsoft Jet database engine version 4.0 file format.|
|**dbVersion120**|Creates a database that uses the Microsoft Access database engine version 12.0 file format.|
If you omit the encryption constant,  **CreateDatabase** creates an un-encrypted database.

Use the  **CreateDatabase** method to create and open a new, empty database, and return the **Database** object. You must complete its structure and content by using additional DAO objects. If you want to make a partial or complete copy of an existing database, you can use the **[CompactDatabase](03f3a156-005a-4b71-81b0-598f326f7d42.md)** method to make a copy that you can customize.


## Example
<a name="sectionSection2"> </a>

This example uses  **CreateDatabase** to create a new, encrypted **Database** object.


```
Sub CreateDatabaseX() 
 
   Dim wrkDefault As Workspace 
   Dim dbsNew As DATABASE 
   Dim prpLoop As Property 
 
   ' Get default Workspace. 
   Set wrkDefault = DBEngine.Workspaces(0) 
 
   ' Make sure there isn't already a file with the name of  
   ' the new database. 
   If Dir("NewDB.mdb") <> "" Then Kill "NewDB.mdb" 
 
   ' Create a new encrypted database with the specified  
   ' collating order. 
   Set dbsNew = wrkDefault.CreateDatabase("NewDB.mdb", _ 
      dbLangGeneral, dbEncrypt) 
 
   With dbsNew 
      Debug.Print "Properties of " &amp; .Name 
      ' Enumerate the Properties collection of the new  
      ' Database object. 
      For Each prpLoop In .Properties 
         If prpLoop <> "" Then Debug.Print "  " &amp; _ 
            prpLoop.Name &amp; " = " &amp; prpLoop 
      Next prpLoop 
   End With 
 
   dbsNew.Close 
 
End Sub 

```

