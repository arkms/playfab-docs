---
author: jasonsandlin
title: "PFPlayerDataManagementClientGetUserReadOnlyDataAsync"
description: "Retrieves the title-specific custom data for the user which can only be read by the client"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 06/20/2023
---

# PFPlayerDataManagementClientGetUserReadOnlyDataAsync  

Retrieves the title-specific custom data for the user which can only be read by the client  

## Syntax  
  
```cpp
HRESULT PFPlayerDataManagementClientGetUserReadOnlyDataAsync(  
    PFEntityHandle entityHandle,  
    const PFPlayerDataManagementGetUserDataRequest* request,  
    XAsyncBlock* async  
)  
```  
  
### Parameters  
  
**`entityHandle`** &nbsp; PFEntityHandle  
  
PFEntityHandle to use for authentication.  
  
**`request`** &nbsp; [PFPlayerDataManagementGetUserDataRequest*](../../pfplayerdatamanagementtypes/structs/pfplayerdatamanagementgetuserdatarequest.md)  
  
Populated request object.  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation.
  
## Remarks  
  
This API is available on all platforms. Data is stored as JSON key-value pairs. Every time the data is updated via any source, the version counter is incremented. If the Version parameter is provided, then this call will only return data if the current version on the system is greater than the value provided. If the Keys parameter is provided, the data object returned will only contain the data specific to the indicated Keys. Otherwise, the full set of custom user data will be returned. See also ClientGetUserDataAsync, ClientUpdateUserDataAsync. When the asynchronous task is complete, call [PFPlayerDataManagementClientGetUserReadOnlyDataGetResultSize](pfplayerdatamanagementclientgetuserreadonlydatagetresultsize.md) and [PFPlayerDataManagementClientGetUserReadOnlyDataGetResult](pfplayerdatamanagementclientgetuserreadonlydatagetresult.md) to get the result.
  
## Requirements  
  
**Header:** PFPlayerDataManagement.h
  
## See also  
[PFPlayerDataManagement members](../pfplayerdatamanagement_members.md)  

  
  
