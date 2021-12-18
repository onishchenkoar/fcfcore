# FSC_CURRENCY_DIM

---

Currency Codes.  Shipped with recent version of the ISO Currency Codes.

| Attribute Name   | Attribute Definition                         | Column Name   | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------|:---------------------------------------------|:--------------|:-------------------|:---------------------|:---------------|:---------------|
| currency_key     | Surrogate key.                               | currency_key  | NUMBER(5)          | Not Null             | Yes            | No             |
| currency_code    | ISO 4217 3 character currency code e.g. USD. | currency_code | CHAR(3)            | Null                 | No             | No             |
| currency_name    | Name of currency e.g. US Dollars.            | currency_name | VARCHAR2(100)      | Null                 | No             | No             |

[Back to index](./README.md)