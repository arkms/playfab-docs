---
author: jasonsandlin
title: "PFAccountManagementServerLinkNintendoServiceAccountSubjectAsync"
description: "Links the Nintendo account associated with the Nintendo Service Account subject or id to the user's PlayFab account"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFAccountManagementServerLinkNintendoServiceAccountSubjectAsync  

Links the Nintendo account associated with the Nintendo Service Account subject or id to the user's PlayFab account  

## Syntax  
  
```cpp
HRESULT PFAccountManagementServerLinkNintendoServiceAccountSubjectAsync(  
    PFEntityHandle titleEntityHandle,  
    const PFAccountManagementLinkNintendoServiceAccountSubjectRequest* request,  
    XAsyncBlock* async  
)  
```  
  
### Parameters  
  
**`titleEntityHandle`** &nbsp; PFEntityHandle  
  
PFEntityHandle for a title Entity obtained using PFAuthenticationGetEntityWithSecretKeyAsync.  
  
**`request`** &nbsp; [PFAccountManagementLinkNintendoServiceAccountSubjectRequest*](../../pfaccountmanagementtypes/structs/pfaccountmanagementlinknintendoserviceaccountsubjectrequest.md)  
  
Populated request object.  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation.
  
## Remarks  
  
This API is available on Win32. See also ServerLinkNintendoServiceAccountAsync, ServerUnlinkNintendoServiceAccountAsync. Call XAsyncGetStatus to get the status of the operation. If the service call is unsuccessful, the async result will be E_PF_INVALID_IDENTITY_PROVIDER_ID, E_PF_LINKED_IDENTIFIER_ALREADY_CLAIMED, E_PF_NINTENDO_SWITCH_NOT_ENABLED_FOR_TITLE or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
## Requirements  
  
**Header:** PFAccountManagement.h
  
## See also  
[PFAccountManagement members](../pfaccountmanagement_members.md)  

  
  
