---
author: jasonsandlin
title: "PFEntityLineageDictionaryEntry"
description: "Dictionary entry for an associative array with PFEntityLineage values."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFEntityLineageDictionaryEntry  

Dictionary entry for an associative array with PFEntityLineage values.  

## Syntax  
  
```cpp
typedef struct PFEntityLineageDictionaryEntry {  
    const char* key;  
    PFEntityLineage const* value;  
} PFEntityLineageDictionaryEntry;  
```
  
### Members  
  
**`key`** &nbsp; const char*  
*is null-terminated*  
  
TBD  
  
**`value`** &nbsp; [PFEntityLineage](pfentitylineage.md) const*  
  
TBD  
  
  
## Requirements  
  
**Header:** PFTypes.h
  
## See also  
[PFTypes members](../pftypes_members.md)  

  
  
