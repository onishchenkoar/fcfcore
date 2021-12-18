# FSC_SUMMARY_TRANS_TYPE_BRIDGE

---

Bridge table to group together transaction types with summary groups.

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TRANSACTION_TYPE_KEY** | Surrogate key for transaction type.                                                    | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PROFILE_SUMMARY_KEY**  | The surrogate key for the profile summary.                                             | NUMBER(12)         | Not Null             | No   | Yes  |
| **CHANGE_CURRENT_IND**   |                                                                                        | CHAR(1)            | Not Null             | No   | No   |
| **CHANGE_END_DATE**      |                                                                                        | DATE               | Not Null             | No   | No   |
| **CHANGE_BEGIN_DATE**    |                                                                                        | DATE               | Null                 | No   | No   |

[Back to index](./index.md)