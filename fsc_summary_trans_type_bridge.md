# FSC_SUMMARY_TRANS_TYPE_BRIDGE

---

Bridge table to group together transaction types with summary groups.

| Attribute Name       | Attribute Definition                                                                   | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:---------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:---------------|:---------------|
| transaction_type_key | Surrogate key for transaction type.                                                    | NUMBER(12)         | Not Null             | No             | Yes            |
| segment_id           | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes            | No             |
| profile_summary_key  | The surrogate key for the profile summary.                                             | NUMBER(12)         | Not Null             | No             | Yes            |
| change_current_ind   |                                                                                        | CHAR(1)            | Not Null             | No             | No             |
| change_end_date      |                                                                                        | DATE               | Not Null             | No             | No             |
| change_begin_date    |                                                                                        | DATE               | Null                 | No             | No             |

[Back to index](./index.md)