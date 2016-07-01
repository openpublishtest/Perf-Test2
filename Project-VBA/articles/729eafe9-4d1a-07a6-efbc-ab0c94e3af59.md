
# Application.CustomFieldIndicatorDelete Method (Project)

Removes a test condition from a custom field graphical indicator criteria list.


## Syntax

 _expression_. **CustomFieldIndicatorDelete**( ** _FieldID_**, ** _Index_**, ** _CriteriaList_** )

 _expression_ A variable that represents an **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _FieldID_|Required|**Long**|The custom field. Can be one of the  **[PjCustomField](eed248af-bde2-8299-3737-253cf96411e2.md)** constants.|
| _Index_|Required|**Integer**|The position of the test condition to delete from the list specified by  **CriteriaList**.|
| _CriteriaList_|Optional|**Long**|The criteria list containing the test condition to be deleted. Can be one of the following  **PjCriteriaList** constants: **pjCriteriaNonSummary**, **pjCriteriaSummary**, or **pjCriteriaProjectSummary**. The default value is **pjCriteriaNonSummary**.|

### Return Value

 **Boolean**


## Remarks

The  **CustomFieldIndicatorDelete** method returns a trappable error (error code 1004) if the list specified by _CriteriaList_ is read-only because it has been set to inherit values from another list.

