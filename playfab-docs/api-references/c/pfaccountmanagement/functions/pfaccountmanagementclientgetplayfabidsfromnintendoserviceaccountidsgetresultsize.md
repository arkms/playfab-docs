---
author: jasonsandlin
title: "PFAccountManagementClientGetPlayFabIDsFromNintendoServiceAccountIdsGetResultSize"
description: "Get the size in bytes needed to store the result of a ClientGetPlayFabIDsFromNintendoServiceAccountIds call."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 07/25/2023
---

# PFAccountManagementClientGetPlayFabIDsFromNintendoServiceAccountIdsGetResultSize  

Get the size in bytes needed to store the result of a ClientGetPlayFabIDsFromNintendoServiceAccountIds call.  

## Syntax  
  
```cpp
HRESULT PFAccountManagementClientGetPlayFabIDsFromNintendoServiceAccountIdsGetResultSize(  
    XAsyncBlock* async,  
    size_t* bufferSize  
)  
```  
  
### Parameters  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
**`bufferSize`** &nbsp; size_t*  
*output*  
  
The buffer size in bytes required for the result.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation. If the service call is unsuccessful, the result will be one of global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
  
## Requirements  
  
**Header:** PFAccountManagement.h
  
## See also  
[PFAccountManagement members](../pfaccountmanagement_members.md)  

  
  
