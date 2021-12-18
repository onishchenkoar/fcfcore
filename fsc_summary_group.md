# FSC_SUMMARY_GROUP

---

Table to hold first level of grouping of transaction types for peer group analysis.  A summary group can have one or more transaction types.

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PROFILE_SUMMARY_KEY**  | The surrogate key for the summary group.                                               | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PROFILE_SUMMARY_ID**   | Summary group identifier.                                                              | VARCHAR2(50)       | Null                 | No   | No   |
| **PROFILE_SUMMARY_NAME** | Summary group name.                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| **PROFILE_SUMMARY_DESC** | Summary group description.                                                             | VARCHAR2(200)      | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**    | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**      | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**   | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)