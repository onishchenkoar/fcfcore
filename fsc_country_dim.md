# FSC_COUNTRY_DIM

---

Country Codes. Shipped with recent version of ISO country codes.

| Attribute Name   | Attribute Definition                     | Column Name    | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------|:-----------------------------------------|:---------------|:-------------------|:---------------------|:---------------|:---------------|
| country_key      | System generated surrogate key..         | country_key    | NUMBER(5)          | Not Null             | Yes            | No             |
| country_code_2   | ISO 2 character country code.  e.g. US.  | country_code_2 | CHAR(2)            | Null                 | No             | No             |
| country_code_3   | ISO 3 character country code.  e.g. USA. | country_code_3 | CHAR(3)            | Null                 | No             | No             |
| country_name     | ISO Country Name..                       | country_name   | VARCHAR2(100)      | Null                 | No             | No             |

[Back to index](./README.md)