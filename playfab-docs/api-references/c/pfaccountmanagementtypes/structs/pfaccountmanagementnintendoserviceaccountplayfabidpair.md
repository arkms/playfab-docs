---
author: jasonsandlin
title: "PFAccountManagementNintendoServiceAccountPlayFabIdPair"
description: "PFAccountManagementNintendoServiceAccountPlayFabIdPair data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 06/26/2023
---

# PFAccountManagementNintendoServiceAccountPlayFabIdPair  

PFAccountManagementNintendoServiceAccountPlayFabIdPair data model.  

## Syntax  
  
```cpp
typedef struct PFAccountManagementNintendoServiceAccountPlayFabIdPair {  
    const char* nintendoServiceAccountId;  
    const char* playFabId;  
} PFAccountManagementNintendoServiceAccountPlayFabIdPair;  
```
  
### Members  
  
**`nintendoServiceAccountId`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) Unique Nintendo Switch Service Account identifier for a user.
  
**`playFabId`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) Unique PlayFab identifier for a user, or null if no PlayFab account is linked to the Nintendo Switch Service Account identifier.
  
  
## Requirements  
  
**Header:** PFAccountManagementTypes.h
  
## See also  
[PFAccountManagementTypes members](../pfaccountmanagementtypes_members.md)  

  
  
