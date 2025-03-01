---
author: jasonsandlin
title: "PFPlayerDataManagementServerGetUserPublisherReadOnlyDataGetResult"
description: "Gets the result of a successful PFPlayerDataManagementServerGetUserPublisherReadOnlyDataAsync call."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 09/25/2023
---

# PFPlayerDataManagementServerGetUserPublisherReadOnlyDataGetResult  

Gets the result of a successful PFPlayerDataManagementServerGetUserPublisherReadOnlyDataAsync call.  

## Syntax  
  
```cpp
HRESULT PFPlayerDataManagementServerGetUserPublisherReadOnlyDataGetResult(  
    XAsyncBlock* async,  
    size_t bufferSize,  
    void* buffer,  
    PFPlayerDataManagementServerGetUserDataResult** result,  
    size_t* bufferUsed  
)  
```  
  
### Parameters  
  
**`async`** &nbsp; XAsyncBlock*  
*_Inout_*  
  
XAsyncBlock for the async operation.  
  
**`bufferSize`** &nbsp; size_t  
  
The size of the buffer for the result object.  
  
**`buffer`** &nbsp; void*  
*_Out_writes_bytes_to_(bufferSize,*bufferUsed)*  
  
Byte buffer used for the result value and its fields.  
  
**`result`** &nbsp; [PFPlayerDataManagementServerGetUserDataResult**](../../pfplayerdatamanagementtypes/structs/pfplayerdatamanagementservergetuserdataresult.md)  
*library-allocated output*  
  
Pointer to the result object.  
  
**`bufferUsed`** &nbsp; size_t*  
*optional output*  
  
The number of bytes in the provided buffer that were used.  
  
  
### Return value
Type: HRESULT
  
Result code for this API operation. If the service call is unsuccessful, the result will be E_PF_PUBLISHER_NOT_SET or any of the global PlayFab Service errors. See doc page "Handling PlayFab Errors" for more details on error handling.
  
## Remarks  
  
result is a pointer within buffer and does not need to be freed separately.
  
## Requirements  
  
**Header:** PFPlayerDataManagement.h
  
## See also  
[PFPlayerDataManagement members](../pfplayerdatamanagement_members.md)  

  
  
