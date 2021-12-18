# FSC_PROFILE_GROUP

---

Table to hold second level of grouping of transaction types for peer group analysis.  A profile group can contain one or more summary groups.

| Attribute Name     | Attribute Definition                                                                   | Column Name        | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:-------------------|:---------------------|:---------------|:---------------|
| profile_group_key  | Surrogate key for profile group.                                                       | profile_group_key  | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id         | VARCHAR2(128)      | Not Null             | Yes            | No             |
| profile_group_id   | Profile group identifier.                                                              | profile_group_id   | VARCHAR2(50)       | Null                 | No             | No             |
| profile_group_name | Profile group name.                                                                    | profile_group_name | VARCHAR2(50)       | Null                 | No             | No             |
| profile_group_desc | Description of the profile group.                                                      | profile_group_desc | VARCHAR2(200)      | Null                 | No             | No             |
| change_begin_date  | Date from which this row was valid.                                                    | change_begin_date  | DATE               | Null                 | No             | No             |
| change_end_date    | Date to which this row was valid.                                                      | change_end_date    | DATE               | Not Null             | No             | No             |
| change_current_ind | Is this the current instance (Y/N).                                                    | change_current_ind | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)