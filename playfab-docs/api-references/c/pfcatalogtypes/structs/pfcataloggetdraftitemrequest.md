---
author: jasonsandlin
title: "PFCatalogGetDraftItemRequest"
description: "PFCatalogGetDraftItemRequest data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFCatalogGetDraftItemRequest  

PFCatalogGetDraftItemRequest data model.  

## Syntax  
  
```cpp
typedef struct PFCatalogGetDraftItemRequest {  
    PFCatalogCatalogAlternateId const* alternateId;  
    PFStringDictionaryEntry const* customTags;  
    uint32_t customTagsCount;  
    PFEntityKey const* entity;  
    const char* id;  
} PFCatalogGetDraftItemRequest;  
```
  
### Members  
  
**`alternateId`** &nbsp; [PFCatalogCatalogAlternateId](pfcatalogcatalogalternateid.md) const*  
*may be nullptr*  
  
(Optional) An alternate ID associated with this item.
  
**`customTags`** &nbsp; [PFStringDictionaryEntry](../../pftypes/structs/pfstringdictionaryentry.md) const*  
*may be nullptr*  
  
(Optional) The optional custom tags associated with the request (e.g. build number, external trace identifiers, etc.).
  
**`customTagsCount`** &nbsp; uint32_t  
  
Count of customTags
  
**`entity`** &nbsp; [PFEntityKey](../../pftypes/structs/pfentitykey-c.md) const*  
*may be nullptr*  
  
(Optional) The entity to perform this action on.
  
**`id`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The unique ID of the item.
  
  
## Requirements  
  
**Header:** PFCatalogTypes.h
  
## See also  
[PFCatalogTypes members](../pfcatalogtypes_members.md)  

  
  
