---
author: jasonsandlin
title: "PFAuthenticationLoginWithXboxGetResult"
description: "Get the result from a PFAuthenticationLoginWithXboxAsync call. The PFEntityHandle will always be returned, but the additional info in the PFAuthenticationLoginResult is only returned if a buffer is provided."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 06/26/2023
---

# PFAuthenticationLoginWithXboxGetResult  

Get the result from a PFAuthenticationLoginWithXboxAsync call. The PFEntityHandle will always be returned, but the additional info in the PFAuthenticationLoginResult is only returned if a buffer is provided.  

## Syntax  
  
```cpp
HRESULT PFAuthenticationLoginWithXboxGetResult(  
    XAsyncBlock* async,  
    PFEntityHandle* entityHandle,  
    size_t bufferSize,  
    void* buffer,  
    PFAuthenticationLoginResult result,  
    size_t* bufferUsed  
)  
```  
  
### Parameters  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
**`entityHandle`** &nbsp; PFEntityHandle*  
*output*  
  
PFEntityHandle which can be used to authenticate other PlayFab API calls.  
  
**`bufferSize`** &nbsp; size_t  
  
The size of the buffer for the result object.  
  
**`buffer`** &nbsp; void*  
*_Out_writes_bytes_to_opt_(bufferSize,*bufferUsed)*  
  
Byte buffer used for the Login result value and its fields.  
  
**`result`** &nbsp; [PFAuthenticationLoginResult](../../pfauthenticationtypes/structs/pfauthenticationloginresult.md)  
*optional, library-allocated output*  
  
Pointer to the LoginResult object.  
  
**`bufferUsed`** &nbsp; size_t*  
*optional output*  
  
The number of bytes in the provided buffer that were used.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation. If the service call is unsuccessful, the result will be E_PF_ENCRYPTION_KEY_MISSING, E_PF_EVALUATION_MODE_PLAYER_COUNT_EXCEEDED, E_PF_EXPIRED_XBOX_LIVE_TOKEN, E_PF_INVALID_XBOX_LIVE_TOKEN, E_PF_REQUEST_VIEW_CONSTRAINT_PARAMS_NOT_ALLOWED, E_PF_SIGNED_REQUEST_NOT_ALLOWED, E_PF_XBOX_INACCESSIBLE, E_PF_XBOX_REJECTED_XSTS_EXCHANGE_REQUEST, E_PF_XBOX_XASS_EXCHANGE_FAILURE or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
## Remarks  
  
If the PFAuthenticationLoginWithXboxAsync call fails, entityHandle with be null. Otherwise, the handle must be closed with PFEntityCloseHandle when it is no longer needed. If returned, 'result' is a pointer within 'buffer' and does not need to be freed separately.
  
## Requirements  
  
**Header:** PFAuthentication.h
  
## See also  
[PFAuthentication members](../pfauthentication_members.md)  

  
  
