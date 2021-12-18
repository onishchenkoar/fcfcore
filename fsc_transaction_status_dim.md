# FSC_TRANSACTION_STATUS_DIM

---

The outcome of a transaction e.g. SUCCESS or FAILURE because EXCEEDED DAILY LIMIT.

| Column Name            | Column Definition               | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:--------------------------------|:-------------------|:---------------------|:-----|:-----|
| transaction_status_key | System generated surrogate key. | NUMBER(5)          | Not Null             | Yes  | No   |
| status_desc            | e.g. SUCCESS, DENIED            | VARCHAR2(20)       | Null                 | No   | No   |
| status_reason_desc     | e.g. EXCEEDED DAILY LIMIT       | VARCHAR2(35)       | Null                 | No   | No   |

[Back to index](./index.md)