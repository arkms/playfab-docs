---
author: jasonsandlin
title: "PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest"
description: "PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 06/26/2023
---

# PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest  

PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest data model.  

## Syntax  
  
```cpp
typedef struct PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest {  
    const char* const* playFabIDs;  
    uint32_t playFabIDsCount;  
} PFAccountManagementGetServerCustomIDsFromPlayFabIDsRequest;  
```
  
### Members  
  
**`playFabIDs`** &nbsp; const char* const*  
  
Array of unique PlayFab player identifiers for which the title needs to get server custom identifiers. Cannot contain more than 25 identifiers.
  
**`playFabIDsCount`** &nbsp; uint32_t  
  
Count of playFabIDs
  
  
## Requirements  
  
**Header:** PFAccountManagementTypes.h
  
## See also  
[PFAccountManagementTypes members](../pfaccountmanagementtypes_members.md)  

  
  
