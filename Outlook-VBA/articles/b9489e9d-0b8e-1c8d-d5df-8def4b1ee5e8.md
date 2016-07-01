
# ExchangeUser Members (Outlook)
Provides detailed information about an  **[AddressEntry](d4a0a85e-8bab-bc56-57bc-d70c3c570c8e.md)** that represents a Microsoft Exchange mailbox user.

Provides detailed information about an  **[AddressEntry](d4a0a85e-8bab-bc56-57bc-d70c3c570c8e.md)** that represents a Microsoft Exchange mailbox user.


## Methods



|**Name**|**Description**|
|:-----|:-----|
|[Delete](d11a82c4-28de-efef-5170-20f999f2bf08.md)|Deletes the  **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object from the **[AddressEntries](db91b717-07c6-d1f2-c545-b766ee1f0c6b.md)** collection object to which it belongs.|
|[Details](6c93a583-cc61-e527-7832-88dba525854a.md)|Displays a modal dialog box that provides detailed information about an  **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object.|
|[GetContact](443fb23a-cd26-e385-bd9d-e978aec56458.md)|Returns  **Null** ( **Nothing** in Visual Basic) because the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object does not correspond to a contact in a Contacts Address Book.|
|[GetDirectReports](753201ad-8001-3185-7d68-fda15907099d.md)|Obtains an  **[AddressEntries](db91b717-07c6-d1f2-c545-b766ee1f0c6b.md)** collection object that contains all the users directly reporting to the Exchange user.|
|[GetExchangeDistributionList](4ebc0448-97a9-ca5c-35f0-ef852de27324.md)|Returns  **Null** ( **Nothing** in Visual Basic) because the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object does not correspond to an **[ExchangeDistributionList](2830dfba-6c0a-a81f-6b98-92ac2aafb59d.md)** object.|
|[GetExchangeUser](ff0babba-895f-8205-fefb-c587ee53ea91.md)|Returns the  **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object.|
|[GetExchangeUserManager](ead5e950-7f7a-b213-0daf-c2bff890a30c.md)|Returns an  **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object that represents the manager of the Exchange user.|
|[GetFreeBusy](0dcd36af-e9d7-ca1e-334f-c540c46254f7.md)|Obtains a  **String** representing the availability of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** for a period of 30 days from the start date, beginning at midnight of the date specified.|
|[GetMemberOfList](1f4e8910-8998-85ab-05dc-d06f6fd323c3.md)|Returns an  **[AddressEntries](db91b717-07c6-d1f2-c545-b766ee1f0c6b.md)** collection object that contains the **[AddressEntry](d4a0a85e-8bab-bc56-57bc-d70c3c570c8e.md)** objects representing all the Exchange distribution lists to which the user belongs.|
|[GetPicture](4298db85-0576-4982-9592-6eae666d966a.md)|Obtains an  **[IPictureDisp](http://msdn.microsoft.com/en-us/library/ms680762%28VS.85%29.aspx)** object that represents the picture of the Microsoft Exchange user that is displayed in Microsoft Outlook.|
|[Update](a2672fbf-f32a-f120-227c-24ee5c361f35.md)|Posts a change to the  **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object in the messaging system.|
|[GetUnifiedGroup](ec0f58fa-969d-ed38-705b-2c99ccbf3c86.md)|Determines if the object is a unified group, by way of a call to [IsUnifiedGroup](46f9564a-1c0a-fe6c-3f06-989fb5f36adf.md).|
|[GetUnifiedGroupFromStore](38a901d3-670f-afd2-a385-3b2bb859cb81.md)|Determines if the object is a unified group, by way of a call to [IsUnifiedGroup](46f9564a-1c0a-fe6c-3f06-989fb5f36adf.md).|
|[IsUnifiedGroup](46f9564a-1c0a-fe6c-3f06-989fb5f36adf.md)|Determines if the object is a unified group.|

## Properties



|**Name**|**Description**|
|:-----|:-----|
|[Address](b3a36b16-e652-9e3f-86fd-7cea0c72d78c.md)|Returns or sets a  **String** representing the X400 e-mail address of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[AddressEntryUserType](fb5b16be-8846-7c9f-22bf-847d2cfc0a54.md)|Returns  **olExchangeUserAddressEntry** which is a constant from the **[OlAddressEntryUserType](9f128fe4-9981-e06a-d69c-ca7cf9107fe9.md)** enumeration representing the user type of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read-only.|
|[Alias](ea87a061-4f09-e0ed-fd3d-bfb44cccaf15.md)|Returns a  **String** representing the alias for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read-only.|
|[Application](17331aa1-d926-ada9-a782-02291cd6f720.md)|Returns an  **[Application](797003e7-ecd1-eccb-eaaf-32d6ddde8348.md)** object that represents the parent application (Outlook) for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object. Read-only.|
|[AssistantName](cca35d99-7031-ba46-4171-8c89b9ea2e2b.md)|Returns a  **String** representing the name of the assistant for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[BusinessTelephoneNumber](c01f85bb-24a2-c08f-df4c-9e6506ca2077.md)|Returns a  **String** representing the business telephone number for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[City](fcec3330-39fb-61e9-e447-4adca0146171.md)|Returns a  **String** representing the city for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[Class](eea4ce34-a957-3771-ae7b-d8fdd959a37d.md)|Returns a constant in the  **[OlObjectClass](33d724b3-df3c-2a7f-a80f-93b66d96f588.md)** enumeration indicating the class of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object. Read-only.|
|[Comments](b55f865c-c564-f209-7648-9977512dd5a5.md)|Returns a  **String** representing the comments for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[CompanyName](d7a630ec-0fbf-78ea-5f2a-51be6d001c23.md)|Returns a  **String** representing the name of the company for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[Department](3b2512ff-d741-53b2-6f1d-a0f74ffbbce1.md)|Returns a  **String** representing the department for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[DisplayType](3060a00b-9a99-7833-1a8a-5c18123d7d98.md)|Returns  **olUser** which is a constant from the **[OlDisplayType](356e5f75-8aa2-e28d-64ee-27b78348ba7a.md)** enumeration representing the nature of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read-only.|
|[FirstName](6a72812a-31fd-aa6a-be08-f765018208ab.md)|Returns a  **String** representing the first name of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[ID](b26ae0d3-ba96-f3ad-cd74-92ce5305e702.md)|Returns a  **String** representing the unique identifier for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read-only.|
|[JobTitle](2cfa5301-3164-c472-3f8e-831c1eebc810.md)|Returns a  **String** representing the job title of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[LastName](1f9f9675-3e72-da56-d654-a1473f4f71a7.md)|Returns a  **String** representing the last name of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[MobileTelephoneNumber](9c76ef68-1f85-d072-11d9-015fbbe1658e.md)|Returns a  **String** representing the mobile telephone number for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[Name](8b93c5a3-7c6a-4193-7fc3-621e1d0dda18.md)|Returns or sets a  **String** value that represents the display name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object. Read/write.|
|[OfficeLocation](b37d5622-27ba-b2c4-cfd3-6aa1e9e9296b.md)|Returns a  **String** representing the office location for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[Parent](18a2505c-14aa-7924-ec59-74c8e85ac92e.md)|Returns the parent  **Object** of the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object. Read-only.|
|[PostalCode](b135d7a6-daa1-4154-d6e7-506c59860a81.md)|Returns a  **String** representing the postal code for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[PrimarySmtpAddress](2dda21da-44a2-fbfe-babc-58646c76689d.md)|Returns a  **String** representing the primary Simple Mail Transfer Protocol (SMTP) address for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read-only.|
|[PropertyAccessor](d1427525-8f6a-04a2-9cfa-b91ee0a89ec2.md)|Returns a  **[PropertyAccessor](2fc91e13-703c-3ec9-9066-ffee7144306c.md)** object that supports creating, getting, setting, and deleting properties of the parent **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** object. Read-only.|
|[Session](7d2d23f0-c441-281a-1784-fe63dfa47b9f.md)|Returns the  **[NameSpace](f0dcaa19-07f5-5d42-a3bf-2e42b7885644.md)** object for the current session. Read-only.|
|[StateOrProvince](abac4889-800a-5573-5851-095f5b5176c5.md)|Returns a  **String** representing the state or province for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[StreetAddress](155399c8-7d99-6537-ba30-84145b26ef21.md)|Returns a  **String** representing the street address for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[Type](de3652a8-023c-5d2c-9ced-88f768c22a87.md)|Returns a  **String** representing the type of entry for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[YomiCompanyName](481fec99-c2ab-c4c7-8e05-ede9e6846d1e.md)|Returns a  **String** representing the Japanese phonetic rendering (yomigana) of the company name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[YomiDepartment](6bc06cf2-7dee-fa50-7380-73df8022ff18.md)|Returns a  **String** representing the Japanese phonetic rendering (yomigana) of the department name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[YomiDisplayName](71e97add-9cf1-86c7-3e94-985d2333ebbd.md)|Returns a  **String** representing the Japanese phonetic rendering (yomigana) of the Exchange display name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[YomiFirstName](b44094df-af5a-21fd-0c09-ada48e51cfd8.md)|Returns a  **String** representing the Japanese phonetic rendering (yomigana) of the first name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
|[YomiLastName](079ba8e7-4a3a-2f8c-fa17-0db5ab8f47c2.md)|Returns a  **String** representing the Japanese phonetic rendering (yomigana) of the last name for the **[ExchangeUser](6ec117d1-7fdb-aa36-b567-1242f8238df0.md)** . Read/write.|
