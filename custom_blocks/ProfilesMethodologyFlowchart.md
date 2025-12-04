---
name: ProfilesMethodologyFlowchart
---
```mermaid
flowchart LR 
 Standardization ---> Profile[Profile Matching] 
 Profile --> Merging[Field Merging]
 Merging --> Normalization[Normalization]
 Normalization --> Location[Geographic Location]
 Location --> Experience[Job History]
 Experience --> Education[Education History]
 Education --> Skills[Skills]
 Skills --> Profiles[Filtered Profiles]
 


```
