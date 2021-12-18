# FSC_PROFILE_SUMMARY_BRIDGE

---

Bridge table to group together summary groups with profile groups.

| Column Name         | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| profile_group_key   | Surrogate key for profile group.                                                       | NUMBER(12)         | Not Null             | No   | Yes  |
| profile_summary_key | The surrogate key for the profile summary.                                             | NUMBER(12)         | Not Null             | No   | Yes  |
| segment_id          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| change_begin_date   |                                                                                        | DATE               | Null                 | No   | No   |
| change_end_date     |                                                                                        | DATE               | Not Null             | No   | No   |
| change_current_ind  |                                                                                        | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)