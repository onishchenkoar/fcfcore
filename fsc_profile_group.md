# FSC_PROFILE_GROUP

---

Table to hold second level of grouping of transaction types for peer group analysis.  A profile group can contain one or more summary groups.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PROFILE_GROUP_KEY**  | Surrogate key for profile group.                                                       | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PROFILE_GROUP_ID**   | Profile group identifier.                                                              | VARCHAR2(50)       | Null                 | No   | No   |
| **PROFILE_GROUP_NAME** | Profile group name.                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| **PROFILE_GROUP_DESC** | Description of the profile group.                                                      | VARCHAR2(200)      | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**  | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND** | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)