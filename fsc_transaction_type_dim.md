# FSC_TRANSACTION_TYPE_DIM

---

A fixed classification of transactions used to analyze transactions in a consistent manner.

[Back to index](./index.md)

| Column Name               | Column Definition                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TRANSACTION_TYPE_KEY**  | Surrogate key                                      | NUMBER(12)         | Not Null             | Yes  | No   |
| **FUNDS_SECURITIES_CODE** | F (funds i.e. money) vs S (securities)             | CHAR(1)            | Null                 | No   | No   |
| **FUNDS_SECURITIES_DESC** | Descriptive version of the code for UI display.    | VARCHAR2(20)       | Null                 | No   | No   |
| **TRANSACTION_CDI_CODE**  | D-Debit, C-Credit, E-Event                         | CHAR(1)            | Null                 | No   | No   |
| **TRANSACTION_CDI_DESC**  | Descriptive version of the code for UI display.    | VARCHAR2(20)       | Null                 | No   | No   |
| **PRIMARY_MEDIUM_DESC**   | e.g. Cash, Check.                                  | VARCHAR2(30)       | Null                 | No   | No   |
| **SECONDARY_MEDIUM_DESC** | e.g. US, non_USD, personal, cashiers, counter etc. | VARCHAR2(30)       | Null                 | No   | No   |
| **MECHANISM_DESC**        | e.g. Teller, ATM, Online                           | VARCHAR2(20)       | Null                 | No   | No   |
| **TERTIARY_MEDIUM_DESC**  | e.g. Fee, Reload, Purchase                         | VARCHAR2(30)       | Null                 | No   | No   |

[Back to index](./index.md)