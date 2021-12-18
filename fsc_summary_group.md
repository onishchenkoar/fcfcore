# FSC_SUMMARY_GROUP

[Back to index](./index.md)

---

Table to hold first level of grouping of transaction types for peer group analysis.  A summary group can have one or more transaction types.

| Column Name          | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| profile_summary_key  | The surrogate key for the summary group.                                               | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| profile_summary_id   | Summary group identifier.                                                              | VARCHAR2(50)       | Null                 | No   | No   |
| profile_summary_name | Summary group name.                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| profile_summary_desc | Summary group description.                                                             | VARCHAR2(200)      | Null                 | No   | No   |
| change_begin_date    | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| change_end_date      | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| change_current_ind   | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)