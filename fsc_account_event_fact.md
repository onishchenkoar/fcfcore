# FSC_ACCOUNT_EVENT_FACT

---

Non-financial account transactoins e.g. Address Change, Beneficiary Change, Account Inquiry.

[Back to index](./index.md)

| Column Name                | Column Definition                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TRANSACTION_KEY**        | Surrogate key                                                                                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to.                                                 | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **BRANCH_KEY**             | Surrogate identifier                                                                                                                   | NUMBER(12)         | Not Null             | No   | Yes  |
| **TIME_KEY**               | System generated surrogate key.  Is NOT of form hhmmss in tables though it does come in that way in the stage files.                   | NUMBER(6)          | Not Null             | No   | Yes  |
| **DATE_KEY**               | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | NUMBER(8,0)        | Not Null             | No   | Yes  |
| **ACCOUNT_KEY**            | System generated surrogate key.                                                                                                        | NUMBER(12)         | Not Null             | No   | Yes  |
| **COUNTRY_KEY**            | System generated surrogate key                                                                                                         | NUMBER(5)          | Not Null             | No   | Yes  |
| **TRANSACTION_TYPE_KEY**   | Surrogate key                                                                                                                          | NUMBER(12)         | Not Null             | No   | Yes  |
| **TRANSACTION_STATUS_KEY** | System generated surrogate key.                                                                                                        | NUMBER(5)          | Not Null             | No   | Yes  |

[Back to index](./index.md)