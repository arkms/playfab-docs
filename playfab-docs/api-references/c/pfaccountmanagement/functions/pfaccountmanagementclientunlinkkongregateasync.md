---
author: jasonsandlin
title: "PFAccountManagementClientUnlinkKongregateAsync"
description: "Unlinks the related Kongregate identifier from the user's PlayFab account"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFAccountManagementClientUnlinkKongregateAsync  

Unlinks the related Kongregate identifier from the user's PlayFab account  

## Syntax  
  
```cpp
HRESULT PFAccountManagementClientUnlinkKongregateAsync(  
    PFEntityHandle entityHandle,  
    const PFAccountManagementUnlinkKongregateAccountRequest* request,  
    XAsyncBlock* async  
)  
```  
  
### Parameters  
  
**`entityHandle`** &nbsp; PFEntityHandle  
  
PFEntityHandle to use for authentication.  
  
**`request`** &nbsp; [PFAccountManagementUnlinkKongregateAccountRequest*](../../pfaccountmanagementtypes/structs/pfaccountmanagementunlinkkongregateaccountrequest.md)  
  
Populated request object.  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation.
  
## Remarks  
  
This API is available on Win32. See also ClientLinkKongregateAsync, ClientLoginWithKongregateAsync. Call XAsyncGetStatus to get the status of the operation. If the service call is unsuccessful, the async result will be E_PF_ACCOUNT_NOT_LINKED or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
## Requirements  
  
**Header:** PFAccountManagement.h
  
## See also  
[PFAccountManagement members](../pfaccountmanagement_members.md)  

  
  
