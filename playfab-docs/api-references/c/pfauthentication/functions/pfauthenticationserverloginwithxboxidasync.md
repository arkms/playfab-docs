---
author: jasonsandlin
title: "PFAuthenticationServerLoginWithXboxIdAsync"
description: "Signs the user in using an Xbox ID and Sandbox ID, returning a session identifier that can subsequently be used for API calls which require an authenticated user"
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFAuthenticationServerLoginWithXboxIdAsync  

Signs the user in using an Xbox ID and Sandbox ID, returning a session identifier that can subsequently be used for API calls which require an authenticated user  

## Syntax  
  
```cpp
HRESULT PFAuthenticationServerLoginWithXboxIdAsync(  
    PFServiceConfigHandle serviceConfigHandle,  
    const char* secretKey,  
    const PFAuthenticationLoginWithXboxIdRequest* request,  
    XAsyncBlock* async  
)  
```  
  
### Parameters  
  
**`serviceConfigHandle`** &nbsp; PFServiceConfigHandle  
  
PFServiceConfigHandle returned from PFServiceConfigCreateHandle call.  
  
**`secretKey`** &nbsp; char*  
*_In_z_*  
  
Title Secret Key used to authenticate the service request.  
  
**`request`** &nbsp; [PFAuthenticationLoginWithXboxIdRequest*](../../pfauthenticationtypes/structs/pfauthenticationloginwithxboxidrequest.md)  
  
Populated request object.  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation.
  
## Remarks  
  
This API is available on Win32. If this is the first time a user has signed in with the Xbox ID and CreateAccount is set to true, a new PlayFab account will be created and linked to the Xbox Live account. In this case, no email or username will be associated with the PlayFab account. Otherwise, if no PlayFab account is linked to the Xbox Live account, an error indicating this will be returned, so that the title can guide the user through creation of a PlayFab account. When the asynchronous task is complete, call [PFAuthenticationServerLoginWithXboxIdGetResult](pfauthenticationserverloginwithxboxidgetresult.md) to get the result.
  
## Requirements  
  
**Header:** PFAuthentication.h
  
## See also  
[PFAuthentication members](../pfauthentication_members.md)  

  
  
