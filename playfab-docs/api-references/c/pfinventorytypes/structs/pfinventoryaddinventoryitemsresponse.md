---
author: jasonsandlin
title: "PFInventoryAddInventoryItemsResponse"
description: "PFInventoryAddInventoryItemsResponse data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFInventoryAddInventoryItemsResponse  

PFInventoryAddInventoryItemsResponse data model.  

## Syntax  
  
```cpp
typedef struct PFInventoryAddInventoryItemsResponse {  
    const char* eTag;  
    const char* idempotencyId;  
    const char* const* transactionIds;  
    uint32_t transactionIdsCount;  
} PFInventoryAddInventoryItemsResponse;  
```
  
### Members  
  
**`eTag`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) ETags are used for concurrency checking when updating resources. More information about using ETags can be found here: https://learn.microsoft.com/gaming/playfab/features/economy-v2/catalog/etags.
  
**`idempotencyId`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The idempotency id used in the request.
  
**`transactionIds`** &nbsp; const char* const*  
*may be nullptr*  
  
(Optional) The ids of transactions that occurred as a result of the request.
  
**`transactionIdsCount`** &nbsp; uint32_t  
  
Count of transactionIds
  
  
## Requirements  
  
**Header:** PFInventoryTypes.h
  
## See also  
[PFInventoryTypes members](../pfinventorytypes_members.md)  

  
  
