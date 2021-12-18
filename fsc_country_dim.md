# **FSC_COUNTRY_DIM**

---

Country Codes. Shipped with recent version of ISO country codes.

[Back to index](./index.md)

| Column Name    | Column Definition                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------|:-----------------------------------------|:-------------------|:---------------------|:-----|:-----|
| country_key    | System generated surrogate key\.         | NUMBER(5)          | Not Null             | Yes  | No   |
| country_code_2 | ISO 2 character country code.  e.g. US.  | CHAR(2)            | Null                 | No   | No   |
| country_code_3 | ISO 3 character country code.  e.g. USA. | CHAR(3)            | Null                 | No   | No   |
| country_name   | ISO Country Name\.                       | VARCHAR2(100)      | Null                 | No   | No   |

[Back to index](./index.md)