# FSC_PROFILE_GROUP

---

Table to hold second level of grouping of transaction types for peer group analysis.  A profile group can contain one or more summary groups.

[Back to index](./index.md)

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| profile_group_key  | Surrogate key for profile group.                                                       | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| profile_group_id   | Profile group identifier.                                                              | VARCHAR2(50)       | Null                 | No   | No   |
| profile_group_name | Profile group name.                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| profile_group_desc | Description of the profile group.                                                      | VARCHAR2(200)      | Null                 | No   | No   |
| change_begin_date  | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| change_end_date    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| change_current_ind | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)