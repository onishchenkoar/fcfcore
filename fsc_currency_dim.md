# FSC_CURRENCY_DIM

[Back to index](./index.md)

---

Currency Codes.  Shipped with recent version of the ISO Currency Codes.

| Column Name   | Column Definition                            | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------|:---------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| currency_key  | Surrogate key.                               | NUMBER(5)          | Not Null             | Yes  | No   |
| currency_code | ISO 4217 3 character currency code e.g. USD. | CHAR(3)            | Null                 | No   | No   |
| currency_name | Name of currency e.g. US Dollars.            | VARCHAR2(100)      | Null                 | No   | No   |

[Back to index](./index.md)