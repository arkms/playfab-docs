---
author: jasonsandlin
title: "PFAccountManagementReportPlayerClientRequest"
description: "PFAccountManagementReportPlayerClientRequest data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFAccountManagementReportPlayerClientRequest  

PFAccountManagementReportPlayerClientRequest data model.  

## Syntax  
  
```cpp
typedef struct PFAccountManagementReportPlayerClientRequest {  
    const char* comment;  
    PFStringDictionaryEntry const* customTags;  
    uint32_t customTagsCount;  
    const char* reporteeId;  
} PFAccountManagementReportPlayerClientRequest;  
```
  
### Members  
  
**`comment`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) Optional additional comment by reporting player.
  
**`customTags`** &nbsp; [PFStringDictionaryEntry](../../pftypes/structs/pfstringdictionaryentry.md) const*  
*may be nullptr*  
  
(Optional) The optional custom tags associated with the request (e.g. build number, external trace identifiers, etc.).
  
**`customTagsCount`** &nbsp; uint32_t  
  
Count of customTags
  
**`reporteeId`** &nbsp; const char*  
*is null-terminated*  
  
Unique PlayFab identifier of the reported player.
  
  
## Requirements  
  
**Header:** PFAccountManagementTypes.h
  
## See also  
[PFAccountManagementTypes members](../pfaccountmanagementtypes_members.md)  

  
  
