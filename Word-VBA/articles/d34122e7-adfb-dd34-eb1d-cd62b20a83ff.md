
# ParagraphFormat Members (Word)
Represents all the formatting for a paragraph.

Represents all the formatting for a paragraph.


## Methods



|**Name**|**Description**|
|:-----|:-----|
|[CloseUp](021ab4fe-3301-90c7-2543-59140b7881da.md)|Removes any spacing before paragraphs in the specified paragraph format.|
|[IndentCharWidth](52e9b6b1-15b3-5e03-7259-21d847c1d59c.md)|Indents one or more paragraphs by a specified number of characters.|
|[IndentFirstLineCharWidth](9531e607-4287-d4a3-de85-315e806d9b51.md)|Indents the first line of one or more paragraphs by a specified number of characters.|
|[OpenOrCloseUp](7cf08077-e3e5-4886-e88f-fd12c2961058.md)|Toggles the spacing before the specified paragraphs.|
|[OpenUp](1473b383-816f-087a-073a-5afc5f530c3a.md)|Sets spacing before the specified paragraphs to 12 points.|
|[Reset](ba44a672-1a02-e673-9bee-b0a7239445a2.md)|Removes manual paragraph formatting (formatting not applied using a style).|
|[Space1](57cc0cea-e50d-affd-1564-30f9240f197b.md)|Single-spaces the specified paragraphs.|
|[Space15](6621d8e8-c207-0862-ddd4-33cb5bcd9cbc.md)|Formats the specified paragraphs with 1.5-line spacing.|
|[Space2](7173f5b8-961b-e93f-e4b6-fedad6da8d1d.md)|Double-spaces the specified paragraphs.|
|[TabHangingIndent](918cec1a-cd94-b2d1-bdbb-99fcbb648947.md)|Sets a hanging indent to a specified number of tab stops. .|
|[TabIndent](db62f9c2-e205-4f57-5baf-2c06bbd30644.md)|Sets the left indent for the specified paragraphs to a specified number of tab stops.|

## Properties



|**Name**|**Description**|
|:-----|:-----|
|[AddSpaceBetweenFarEastAndAlpha](3575dab1-4a59-b20e-46e2-971389a3ec95.md)| **True** if Microsoft Word is set to automatically add spaces between Japanese and Latin text for the specified paragraphs. This property returns **wdUndefined** if it's set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[AddSpaceBetweenFarEastAndDigit](9792aa0e-bb31-463b-ef7c-99847f587c19.md)| **True** if Microsoft Word is set to automatically add spaces between Japanese text and numbers for the specified paragraphs. This property returns **wdUndefined** if it's set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[Alignment](637e83e0-813e-1a8d-18f2-6a8d41dc47af.md)|Returns or sets a  **WdParagraphAlignment** constant that represents the alignment for the specified paragraphs. Read/write.|
|[Application](7baa80b6-c8dc-ea6e-efed-0e577123a0a9.md)|Returns an  **[Application](d1cf6f8f-4e88-bf01-93b4-90a83f79cb44.md)** object that represents the Microsoft Word application.|
|[AutoAdjustRightIndent](7897e1c5-9bc8-93af-878e-c1670f066b33.md)| **True** if Microsoft Word is set to automatically adjust the right indent for the specified paragraphs if you've specified a set number of characters per line. Returns **wdUndefined** if the **AutoAdjustRightIndent** property is set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[BaseLineAlignment](857b29f2-7a31-27fb-4802-910470a6656b.md)|Returns or sets a  **WdBaselineAlignment** constant that represents the vertical position of fonts on a line. Read/write.|
|[Borders](d8c57d5b-1c7a-2710-503c-a671ddae0dc7.md)|Returns a  **[Borders](6dd1d4cc-2dcf-22c7-a299-4721a5543ba3.md)** collection that represents all the borders for the specified object.|
|[CharacterUnitFirstLineIndent](f5e68ef0-7086-4d33-7ed0-3c0569d203cd.md)|Returns or sets the value (in characters) for a first-line or hanging indent. Use a positive value to set a first-line indent, and use a negative value to set a hanging indent. Read/write  **Single** .|
|[CharacterUnitLeftIndent](b54132c9-3d4a-a8d5-2778-c01928f5dda5.md)|Returns or sets the left indent value (in characters) for the specified paragraphs. Read/write  **Single** .|
|[CharacterUnitRightIndent](ef9476ce-fa19-3c75-934b-9dd33da23076.md)|Returns or sets the right indent value (in characters) for the specified paragraphs. Read/write  **Single** .|
|[CollapsedByDefault](50a0adf5-1229-4e79-0acb-d8461a3ecc94.md)|Returns or sets whether the specified paragraph format is collapsed by default. Read-write  **Long**.|
|[Creator](500803c4-b7f8-0a99-6e96-4f783698725f.md)|Returns a 32-bit integer that indicates the application in which the specified object was created. Read-only  **Long** .|
|[DisableLineHeightGrid](8cb667e6-ce9c-8b1e-253e-bad67032ed72.md)| **True** if Microsoft Word aligns characters in the specified paragraphs to the line grid when a set number of lines per page is specified. Returns **wdUndefined** if the **DisableLineHeightGrid** property is set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[Duplicate](cc5e9633-ea7c-8317-5321-c7bbf1288579.md)|Returns a read-only  **ParagraphFormat** object that represents the paragraph formatting of the specified paragraph.|
|[FarEastLineBreakControl](554a0097-5402-2b40-face-c9ec942ad3e1.md)| **True** if Microsoft Word applies East Asian line-breaking rules to the specified paragraphs. Returns **wdUndefined** if the **FarEastLineBreakControl** property is set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[FirstLineIndent](a9a94019-537c-942d-c388-06b228fd5463.md)|Returns or sets the value (in points) for a first line or hanging indent. Use a positive value to set a first-line indent, and use a negative value to set a hanging indent. Read/write  **Single** .|
|[HalfWidthPunctuationOnTopOfLine](f4b2a723-ec3c-d8bd-eb82-66423399c549.md)| **True** if Microsoft Word changes punctuation symbols at the beginning of a line to half-width characters for the specified paragraphs. This property returns **wdUndefined** if it's set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[HangingPunctuation](9dc481f6-65fd-35f3-0765-087996aa6564.md)| **True** if hanging punctuation is enabled for the specified paragraphs. This property returns **wdUndefined** if it's set to **True** for only some of the specified paragraphs. Read/write **Long** .|
|[Hyphenation](185d00c0-3f19-bc98-9790-823b49d289b1.md)| **True** if the specified paragraphs are included in automatic hyphenation. **False** if the specified paragraphs are to be excluded from automatic hyphenation. Read/write **Long** .|
|[KeepTogether](7cc4cade-f986-8dad-a1b3-e1fade4c6825.md)| **True** if all lines in the specified paragraphs remain on the same page when Microsoft Word repaginates the document. Read/write **Long** .|
|[KeepWithNext](5fc8ad97-d839-7837-04c7-dac2efe1d1c2.md)| **True** if the specified paragraph remains on the same page as the paragraph that follows it when Microsoft Word repaginates the document. Read/write **Long** .|
|[LeftIndent](bbd102d3-8263-a7ec-6909-518ab9e88a8f.md)|Returns or sets a  **Single** that represents the left indent value (in points) for the specified paragraph formatting. Read/write.|
|[LineSpacing](30d067e2-9802-f119-bc4c-bd31bfe187f5.md)|Returns or sets the line spacing (in points) for the specified paragraphs. Read/write  **Single** .|
|[LineSpacingRule](a08e9eeb-1b85-7cd8-a497-ac7d63234267.md)|Returns or sets the line spacing for the specified paragraph formatting. Read/write  **[WdLineSpacing](02e95bf9-b295-2199-a5cf-a7798b1273a0.md)** .|
|[LineUnitAfter](243cde4f-8bcb-1be6-0885-ffaf0bbe83d1.md)|Returns or sets the amount of spacing (in gridlines) after the specified paragraphs. Read/write  **Single** .|
|[LineUnitBefore](05ad3a0e-acc6-dc42-640c-eafabae1d391.md)|Returns or sets the amount of spacing (in gridlines) before the specified paragraphs. Read/write  **Single** .|
|[MirrorIndents](51521bd0-f492-c83c-1688-04779fa5cd53.md)|Returns or sets a  **Long** that represents whether left and right indents are the same width. Can be **True** , **False** , or **wdUndefined** . Read/write.|
|[NoLineNumber](49116752-3c3a-d61c-6d54-2dbca5e902f1.md)| **True** if line numbers are repressed for the specified paragraphs. Can be **True** , **False** , or **wdUndefined** . Read/write **Long** .|
|[OutlineLevel](e1356015-636e-87c3-a6c7-f765276a6079.md)|Returns or sets the outline level for the specified paragraphs. Read/write  **[WdOutlineLevel](44a38f7e-355c-3ff3-1408-0972f20778d2.md)** .|
|[PageBreakBefore](b024b5a6-4207-c490-97a6-a5eb2903c90e.md)| **True** if a page break is forced before the specified paragraphs. Can be **True** , **False** , or **wdUndefined** . Read/write **Long** .|
|[Parent](fdc51dcf-3d40-9c24-a7de-4d69cc8e98ed.md)|Returns an  **Object** that represents the parent object of the specified **ParagraphFormat** object.|
|[ReadingOrder](4a22e638-2af8-096a-d45c-2eed21dc8002.md)|Returns or sets the reading order of the specified paragraphs without changing their alignment. Read/write  **WdReadingOrder** .|
|[RightIndent](de69209e-d88d-d367-9d84-94faa07a30bd.md)|Returns or sets the right indent (in points) for the specified paragraphs. Read/write  **Single** .|
|[Shading](20e67a80-15ca-8b9b-d565-6e7c79a6ea14.md)|Returns a  **[Shading](e136509a-1be1-29e4-7b37-1faf659e37ba.md)** object that refers to the shading formatting for the specified object.|
|[SpaceAfter](804ffaf6-8a74-22a1-7a90-132847b196ee.md)|Returns or sets the amount of spacing (in points) after the specified paragraph or text column. Read/write  **Single** .|
|[SpaceAfterAuto](c54c024a-5c04-fca5-95cb-bcbadb4baf41.md)| **True** if Microsoft Word automatically sets the amount of spacing after the specified paragraphs. Read/write **Long** .|
|[SpaceBefore](da20b86e-b69c-f7df-cbaa-46f208ddbdc9.md)|Returns or sets the spacing (in points) before the specified paragraphs. Read/write  **Single** .|
|[SpaceBeforeAuto](c3c86ee1-c62f-d921-2dc7-d7201b181622.md)| **True** if Microsoft Word automatically sets the amount of spacing before the specified paragraphs. Read/write **Long** .|
|[Style](81da5d84-32e6-e133-4f2c-a7652b0356b1.md)|Returns or sets the style for the specified object. Read/write  **Variant** .|
|[TabStops](9eed85b9-aee6-04af-c5ce-f6ba47176d35.md)|Returns or sets a  **TabStops** collection that represents all the custom tab stops for the specified paragraphs. Read/write.|
|[TextboxTightWrap](0831db5c-4454-75ca-e52b-1ba79efd40be.md)|Returns or sets a  **[WdTextboxTightWrap](6d9e0dcd-816a-e055-b96a-7da5dcea38f7.md)** constant that represents how tightly text wraps around shapes or text boxes. Read/write.|
|[WidowControl](461a8d5f-2f64-b3c4-657b-0b592c482ac0.md)| **True** if the first and last lines in the specified paragraph remain on the same page as the rest of the paragraph when Word repaginates the document. Can be **True** , **False** or **wdUndefined** . Read/write **Long** .|
|[WordWrap](da5e67c3-405d-8adb-5cec-321464030f08.md)| **True** if Microsoft Word wraps Latin text in the middle of a word in the specified paragraphs or text frames. Read/write **Long** .|
