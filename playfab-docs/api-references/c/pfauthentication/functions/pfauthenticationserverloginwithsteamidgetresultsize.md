---
author: jasonsandlin
title: "PFAuthenticationServerLoginWithSteamIdGetResultSize"
description: "Get the size in bytes needed to store the result of a PFAuthenticationServerLoginWithSteamIdAsync call."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFAuthenticationServerLoginWithSteamIdGetResultSize  

Get the size in bytes needed to store the result of a PFAuthenticationServerLoginWithSteamIdAsync call.  

## Syntax  
  
```cpp
HRESULT PFAuthenticationServerLoginWithSteamIdGetResultSize(  
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
  
Result code for this API operation. If the service call is unsuccessful, the result will be E_PF_EVALUATION_MODE_PLAYER_COUNT_EXCEEDED, E_PF_REQUEST_VIEW_CONSTRAINT_PARAMS_NOT_ALLOWED, E_PF_STEAM_NOT_ENABLED_FOR_TITLE, E_PF_STEAM_USER_NOT_FOUND or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
  
## Requirements  
  
**Header:** PFAuthentication.h
  
## See also  
[PFAuthentication members](../pfauthentication_members.md)  

  
  
