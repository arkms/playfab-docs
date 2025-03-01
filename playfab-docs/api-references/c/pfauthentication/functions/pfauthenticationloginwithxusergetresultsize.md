---
author: jasonsandlin
title: "PFAuthenticationLoginWithXUserGetResultSize"
description: "Get the size in bytes needed to store the result of a PFAuthenticationLoginWithXUserAsync call."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFAuthenticationLoginWithXUserGetResultSize  

Get the size in bytes needed to store the result of a PFAuthenticationLoginWithXUserAsync call.  

## Syntax  
  
```cpp
HRESULT PFAuthenticationLoginWithXUserGetResultSize(  
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
  
Result code for this API operation. If the service call is unsuccessful, the result will be E_PF_ENCRYPTION_KEY_MISSING, E_PF_EVALUATION_MODE_PLAYER_COUNT_EXCEEDED, E_PF_EXPIRED_XBOX_LIVE_TOKEN, E_PF_INVALID_XBOX_LIVE_TOKEN, E_PF_REQUEST_VIEW_CONSTRAINT_PARAMS_NOT_ALLOWED, E_PF_SIGNED_REQUEST_NOT_ALLOWED, E_PF_XBOX_INACCESSIBLE, E_PF_XBOX_REJECTED_XSTS_EXCHANGE_REQUEST, E_PF_XBOX_XASS_EXCHANGE_FAILURE or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
  
## Requirements  
  
**Header:** PFAuthentication.h
  
## See also  
[PFAuthentication members](../pfauthentication_members.md)  

  
  
