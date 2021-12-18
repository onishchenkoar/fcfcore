# FSC_CURRENCY_DIM

---

Currency Codes.  Shipped with recent version of the ISO Currency Codes.

[Back to index](./index.md)

| Column Name       | Column Definition                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------|:---------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CURRENCY_KEY**  | Surrogate key.                               | NUMBER(5)          | Not Null             | Yes  | No   |
| **CURRENCY_CODE** | ISO 4217 3 character currency code e.g. USD. | CHAR(3)            | Null                 | No   | No   |
| **CURRENCY_NAME** | Name of currency e.g. US Dollars.            | VARCHAR2(100)      | Null                 | No   | No   |

[Back to index](./index.md)