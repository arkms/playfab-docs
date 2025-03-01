---
author: jasonsandlin
title: "PFPlayerDataManagementServerUpdateUserReadOnlyDataAsync"
description: "Updates the title-specific custom data for the user which can only be read by the client"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFPlayerDataManagementServerUpdateUserReadOnlyDataAsync  

Updates the title-specific custom data for the user which can only be read by the client  

## Syntax  
  
```cpp
HRESULT PFPlayerDataManagementServerUpdateUserReadOnlyDataAsync(  
    PFEntityHandle titleEntityHandle,  
    const PFPlayerDataManagementServerUpdateUserDataRequest* request,  
    XAsyncBlock* async  
)  
```  
  
### Parameters  
  
**`titleEntityHandle`** &nbsp; PFEntityHandle  
  
PFEntityHandle for a title Entity obtained using PFAuthenticationGetEntityWithSecretKeyAsync.  
  
**`request`** &nbsp; [PFPlayerDataManagementServerUpdateUserDataRequest*](../../pfplayerdatamanagementtypes/structs/pfplayerdatamanagementserverupdateuserdatarequest.md)  
  
Populated request object.  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation.
  
## Remarks  
  
This API is available on Win32. This function performs an additive update of the arbitrary JSON object containing the custom data for the user. In updating the custom data object, keys which already exist in the object will have their values overwritten, keys with null values will be removed. No other key-value pairs will be changed apart from those specified in the call. See also ServerGetUserDataAsync, ServerGetUserInternalDataAsync, ServerGetUserReadOnlyDataAsync, ServerUpdateUserDataAsync, ServerUpdateUserInternalDataAsync. When the asynchronous task is complete, call [PFPlayerDataManagementServerUpdateUserReadOnlyDataGetResult](pfplayerdatamanagementserverupdateuserreadonlydatagetresult.md) to get the result.
  
## Requirements  
  
**Header:** PFPlayerDataManagement.h
  
## See also  
[PFPlayerDataManagement members](../pfplayerdatamanagement_members.md)  

  
  
