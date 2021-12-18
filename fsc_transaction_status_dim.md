# FSC_TRANSACTION_STATUS_DIM

---

The outcome of a transaction e.g. SUCCESS or FAILURE because EXCEEDED DAILY LIMIT.

[Back to index](./index.md)

| Column Name                | Column Definition               | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:--------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TRANSACTION_STATUS_KEY** | System generated surrogate key. | NUMBER(5)          | Not Null             | Yes  | No   |
| **STATUS_DESC**            | e.g. SUCCESS, DENIED            | VARCHAR2(20)       | Null                 | No   | No   |
| **STATUS_REASON_DESC**     | e.g. EXCEEDED DAILY LIMIT       | VARCHAR2(35)       | Null                 | No   | No   |

[Back to index](./index.md)