# FSC_TRANSACTION_TYPE_DIM

---

A fixed classification of transactions used to analyze transactions in a consistent manner.

| Column Name           | Column Definition                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:---------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| transaction_type_key  | Surrogate key                                      | NUMBER(12)         | Not Null             | Yes  | No   |
| funds_securities_code | F (funds i.e. money) vs S (securities)             | CHAR(1)            | Null                 | No   | No   |
| funds_securities_desc | Descriptive version of the code for UI display.    | VARCHAR2(20)       | Null                 | No   | No   |
| transaction_cdi_code  | D-Debit, C-Credit, E-Event                         | CHAR(1)            | Null                 | No   | No   |
| transaction_cdi_desc  | Descriptive version of the code for UI display.    | VARCHAR2(20)       | Null                 | No   | No   |
| primary_medium_desc   | e.g. Cash, Check.                                  | VARCHAR2(30)       | Null                 | No   | No   |
| secondary_medium_desc | e.g. US, non_USD, personal, cashiers, counter etc. | VARCHAR2(30)       | Null                 | No   | No   |
| mechanism_desc        | e.g. Teller, ATM, Online                           | VARCHAR2(20)       | Null                 | No   | No   |
| tertiary_medium_desc  | e.g. Fee, Reload, Purchase                         | VARCHAR2(30)       | Null                 | No   | No   |

[Back to index](./index.md)