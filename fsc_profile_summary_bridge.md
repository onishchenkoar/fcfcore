# FSC_PROFILE_SUMMARY_BRIDGE

---

Bridge table to group together summary groups with profile groups.

| Attribute Name      | Attribute Definition                                                                   | Column Name        | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:--------------------|:---------------------------------------------------------------------------------------|:-------------------|:-------------------|:---------------------|:---------------|:---------------|
| profile_group_key   | Surrogate key for profile group.                                                       | profile_group_key  | NUMBER(12)         | Not Null             | No             | Yes            |
| profile_summary_key | The surrogate key for the profile summary.                                             | summary_group_key  | NUMBER(12)         | Not Null             | No             | Yes            |
| segment_id          | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id         | VARCHAR2(128)      | Not Null             | Yes            | No             |
| change_begin_date   |                                                                                        | change_begin_date  | DATE               | Null                 | No             | No             |
| change_end_date     |                                                                                        | change_end_date    | DATE               | Not Null             | No             | No             |
| change_current_ind  |                                                                                        | change_current_ind | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)