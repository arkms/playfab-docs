---
author: jasonsandlin
title: "PFSegmentsContactEmailInfo"
description: "PFSegmentsContactEmailInfo data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFSegmentsContactEmailInfo  

PFSegmentsContactEmailInfo data model.  

## Syntax  
  
```cpp
typedef struct PFSegmentsContactEmailInfo {  
    const char* emailAddress;  
    const char* name;  
    PFEmailVerificationStatus const* verificationStatus;  
} PFSegmentsContactEmailInfo;  
```
  
### Members  
  
**`emailAddress`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The email address.
  
**`name`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The name of the email info data.
  
**`verificationStatus`** &nbsp; [PFEmailVerificationStatus](../../pftypes/enums/pfemailverificationstatus.md) const*  
*may be nullptr*  
  
(Optional) The verification status of the email.
  
  
## Requirements  
  
**Header:** PFSegmentsTypes.h
  
## See also  
[PFSegmentsTypes members](../pfsegmentstypes_members.md)  

  
  
