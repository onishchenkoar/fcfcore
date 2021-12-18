# FSC_ACCOUNT_EVENT_FACT

---

Non-financial account transactoins e.g. Address Change, Beneficiary Change, Account Inquiry.

| Attribute Name         | Attribute Definition                                                                                                                   | Column Name            | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-----------------------|:-------------------|:---------------------|:---------------|:---------------|
| transaction_key        | Surrogate key                                                                                                                          | transaction_key        | NUMBER(12)         | Not Null             | No             | Yes            |
| segment_id             | Multibank configurations use this column to indicate which bank the record belongs to.                                                 | segment_id             | VARCHAR2(128)      | Not Null             | No             | Yes            |
| branch_key             | Surrogate identifier                                                                                                                   | branch_key             | NUMBER(12)         | Not Null             | No             | Yes            |
| time_key               | System generated surrogate key.  Is NOT of form hhmmss in tables though it does come in that way in the stage files.                   | time_key               | NUMBER(6)          | Not Null             | No             | Yes            |
| date_key               | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | date_key               | NUMBER(8,0)        | Not Null             | No             | Yes            |
| account_key            | System generated surrogate key.                                                                                                        | account_key            | NUMBER(12)         | Not Null             | No             | Yes            |
| country_key            | System generated surrogate key                                                                                                         | country_key            | NUMBER(5)          | Not Null             | No             | Yes            |
| transaction_type_key   | Surrogate key                                                                                                                          | transaction_type_key   | NUMBER(12)         | Not Null             | No             | Yes            |
| transaction_status_key | System generated surrogate key.                                                                                                        | transaction_status_key | NUMBER(5)          | Not Null             | No             | Yes            |

[Back to index](./README.md)