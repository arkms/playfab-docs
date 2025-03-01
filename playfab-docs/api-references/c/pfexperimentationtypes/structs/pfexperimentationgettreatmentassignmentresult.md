---
author: jasonsandlin
title: "PFExperimentationGetTreatmentAssignmentResult"
description: "PFExperimentationGetTreatmentAssignmentResult data model."
ms.author: jasonsa
ms.topic: reference
ms.service: playfab
ms.date: 05/24/2023
---

# PFExperimentationGetTreatmentAssignmentResult  

PFExperimentationGetTreatmentAssignmentResult data model.  

## Syntax  
  
```cpp
typedef struct PFExperimentationGetTreatmentAssignmentResult {  
    PFTreatmentAssignment const* treatmentAssignment;  
} PFExperimentationGetTreatmentAssignmentResult;  
```
  
### Members  
  
**`treatmentAssignment`** &nbsp; [PFTreatmentAssignment](../../pftypes/structs/pftreatmentassignment.md) const*  
*may be nullptr*  
  
(Optional) Treatment assignment for the entity.
  
  
## Requirements  
  
**Header:** PFExperimentationTypes.h
  
## See also  
[PFExperimentationTypes members](../pfexperimentationtypes_members.md)  

  
  
