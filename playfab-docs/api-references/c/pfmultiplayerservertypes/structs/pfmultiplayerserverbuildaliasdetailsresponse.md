---
author: jasonsandlin
title: "PFMultiplayerServerBuildAliasDetailsResponse"
description: "PFMultiplayerServerBuildAliasDetailsResponse data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFMultiplayerServerBuildAliasDetailsResponse  

PFMultiplayerServerBuildAliasDetailsResponse data model.  

## Syntax  
  
```cpp
typedef struct PFMultiplayerServerBuildAliasDetailsResponse {  
    const char* aliasId;  
    const char* aliasName;  
    PFMultiplayerServerBuildSelectionCriterion const* buildSelectionCriteria;  
    uint32_t buildSelectionCriteriaCount;  
} PFMultiplayerServerBuildAliasDetailsResponse;  
```
  
### Members  
  
**`aliasId`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The guid string alias Id of the alias to be created or updated.
  
**`aliasName`** &nbsp; const char*  
*is null-terminated*  
  
(Optional) The alias name.
  
**`buildSelectionCriteria`** &nbsp; [PFMultiplayerServerBuildSelectionCriterion](pfmultiplayerserverbuildselectioncriterion.md) const*  
*may be nullptr*  
  
(Optional) Array of build selection criteria.
  
**`buildSelectionCriteriaCount`** &nbsp; uint32_t  
  
Count of buildSelectionCriteria
  
  
## Requirements  
  
**Header:** PFMultiplayerServerTypes.h
  
## See also  
[PFMultiplayerServerTypes members](../pfmultiplayerservertypes_members.md)  

  
  
