# FSC_HOUSEHOLD_ACCOUNT_BRIDGE

---

Which accounts are in which households.  This is derived from the household-party and party-account bridges.

[Back to index](./index.md)

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| household_key      | System generated surrogate identifier\.                                                | NUMBER(12)         | Not Null             | No   | Yes  |
| account_key        | System generated surrogate key.                                                        | NUMBER(12)         | Not Null             | No   | Yes  |
| change_begin_date  | Date from which this row was valid.                                                    | DATE               | Not Null             | Yes  | No   |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | No   | Yes  |
| change_end_date    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| change_current_ind | Is this the current instance (Y/N)                                                     | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)