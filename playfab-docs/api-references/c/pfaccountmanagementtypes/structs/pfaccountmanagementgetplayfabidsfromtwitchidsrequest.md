---
author: jasonsandlin
title: "PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest"
description: "PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 06/26/2023
---

# PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest  

PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest data model.  

## Syntax  
  
```cpp
typedef struct PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest {  
    const char* const* twitchIds;  
    uint32_t twitchIdsCount;  
} PFAccountManagementGetPlayFabIDsFromTwitchIDsRequest;  
```
  
### Members  
  
**`twitchIds`** &nbsp; const char* const*  
  
Array of unique Twitch identifiers (Twitch's _id) for which the title needs to get PlayFab identifiers. The array cannot exceed 2,000 in length.
  
**`twitchIdsCount`** &nbsp; uint32_t  
  
Count of twitchIds
  
  
## Requirements  
  
**Header:** PFAccountManagementTypes.h
  
## See also  
[PFAccountManagementTypes members](../pfaccountmanagementtypes_members.md)  

  
  
