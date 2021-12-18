# FSC_PROFILE_SUMMARY_BRIDGE

---

Bridge table to group together summary groups with profile groups.

[Back to index](./index.md)

| Column Name             | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PROFILE_GROUP_KEY**   | Surrogate key for profile group.                                                       | NUMBER(12)         | Not Null             | No   | Yes  |
| **PROFILE_SUMMARY_KEY** | The surrogate key for the profile summary.                                             | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CHANGE_BEGIN_DATE**   |                                                                                        | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**     |                                                                                        | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**  |                                                                                        | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)