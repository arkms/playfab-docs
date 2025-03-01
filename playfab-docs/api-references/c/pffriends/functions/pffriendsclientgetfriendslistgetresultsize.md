---
author: jasonsandlin
title: "PFFriendsClientGetFriendsListGetResultSize"
description: "Get the size in bytes needed to store the result of a ClientGetFriendsList call."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFFriendsClientGetFriendsListGetResultSize  

Get the size in bytes needed to store the result of a ClientGetFriendsList call.  

## Syntax  
  
```cpp
HRESULT PFFriendsClientGetFriendsListGetResultSize(  
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
  
Result code for this API operation. If the service call is unsuccessful, the result will be E_PF_ACCOUNT_NOT_FOUND, E_PF_EXPIRED_XBOX_LIVE_TOKEN, E_PF_FACEBOOK_API_ERROR, E_PF_INVALID_XBOX_LIVE_TOKEN, E_PF_XBOX_INACCESSIBLE, E_PF_XBOX_SERVICE_TOO_MANY_REQUESTS, E_PF_XBOX_XASS_EXCHANGE_FAILURE or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
  
## Requirements  
  
**Header:** PFFriends.h
  
## See also  
[PFFriends members](../pffriends_members.md)  

  
  
