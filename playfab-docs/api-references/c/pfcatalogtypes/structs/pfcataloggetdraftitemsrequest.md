---
author: jasonsandlin
title: "PFCatalogGetDraftItemsRequest"
description: "PFCatalogGetDraftItemsRequest data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFCatalogGetDraftItemsRequest  

PFCatalogGetDraftItemsRequest data model.  

## Syntax  
  
```cpp
typedef struct PFCatalogGetDraftItemsRequest {  
    PFCatalogCatalogAlternateId const* alternateIds;  
    uint32_t alternateIdsCount;  
    PFStringDictionaryEntry const* customTags;  
    uint32_t customTagsCount;  
    PFEntityKey const* entity;  
    const char* const* ids;  
    uint32_t idsCount;  
} PFCatalogGetDraftItemsRequest;  
```
  
### Members  
  
**`alternateIds`** &nbsp; [PFCatalogCatalogAlternateId](pfcatalogcatalogalternateid.md) const*  
*may be nullptr*  
  
(Optional) List of item alternate IDs.
  
**`alternateIdsCount`** &nbsp; uint32_t  
  
Count of alternateIds
  
**`customTags`** &nbsp; [PFStringDictionaryEntry](../../pftypes/structs/pfstringdictionaryentry.md) const*  
*may be nullptr*  
  
(Optional) The optional custom tags associated with the request (e.g. build number, external trace identifiers, etc.).
  
**`customTagsCount`** &nbsp; uint32_t  
  
Count of customTags
  
**`entity`** &nbsp; [PFEntityKey](../../pftypes/structs/pfentitykey-c.md) const*  
*may be nullptr*  
  
(Optional) The entity to perform this action on.
  
**`ids`** &nbsp; const char* const*  
*may be nullptr*  
  
(Optional) List of Item Ids.
  
**`idsCount`** &nbsp; uint32_t  
  
Count of ids
  
  
## Requirements  
  
**Header:** PFCatalogTypes.h
  
## See also  
[PFCatalogTypes members](../pfcatalogtypes_members.md)  

  
  
