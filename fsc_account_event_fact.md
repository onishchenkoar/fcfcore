# FSC_ACCOUNT_EVENT_FACT

---

Non-financial account transactoins e.g. Address Change, Beneficiary Change, Account Inquiry.

| Column Name            | Column Definition                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| transaction_key        | Surrogate key                                                                                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| segment_id             | Multibank configurations use this column to indicate which bank the record belongs to.                                                 | VARCHAR2(128)      | Not Null             | No   | Yes  |
| branch_key             | Surrogate identifier                                                                                                                   | NUMBER(12)         | Not Null             | No   | Yes  |
| time_key               | System generated surrogate key.  Is NOT of form hhmmss in tables though it does come in that way in the stage files.                   | NUMBER(6)          | Not Null             | No   | Yes  |
| date_key               | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | NUMBER(8,0)        | Not Null             | No   | Yes  |
| account_key            | System generated surrogate key.                                                                                                        | NUMBER(12)         | Not Null             | No   | Yes  |
| country_key            | System generated surrogate key                                                                                                         | NUMBER(5)          | Not Null             | No   | Yes  |
| transaction_type_key   | Surrogate key                                                                                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| transaction_status_key | System generated surrogate key.                                                                                                        | NUMBER(5)          | Not Null             | No   | Yes  |

[Back to index](./index.md)