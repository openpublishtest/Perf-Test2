
# Document.FooterMargin Property (Visio)

Gets or sets the margin of a document's footer. Read/write.


## Syntax

 _expression_ . **FooterMargin**( **_UnitsNameOrCode_** )

 _expression_ A variable that represents a **Document** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _UnitsNameOrCode_|Optional| **Variant**|The units to use when retrieving or setting the cell's value. Defaults to internal drawing units (inches).|

### Return Value

Double


## Remarks

If UnitsNameOrCode is not provided, the  **FooterMargin** property will default to internal drawing units.

You can also set this value in the  **Margin** box under **Footer** in the **Header and Footer** dialog box (click the **File** tab, click **Print**, click  **Print Preview**, and then in the  **Preview** group, click **Header &amp; Footer**).

Automation constants for representing units are declared by the Microsoft Visio type library in member  **[VisUnitCodes](fce91c1b-d5c2-6522-2446-0b8f6cacbc84.md)** .

For a complete list of valid unit strings along with corresponding Automation constants (integer values), see [About Units of Measure](http://msdn.microsoft.com/library/b6140312-b8e6-0cf2-9fe0-b14e800216bf%28Office.15%29.aspx).

