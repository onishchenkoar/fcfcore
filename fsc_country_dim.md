# FSC_COUNTRY_DIM

---

Country Codes. Shipped with recent version of ISO country codes.

[Back to index](./index.md)

| Column Name        | Column Definition                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:-----------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **COUNTRY_KEY**    | System generated surrogate key\.         | NUMBER(5)          | Not Null             | Yes  | No   |
| **COUNTRY_CODE_2** | ISO 2 character country code.  e.g. US.  | CHAR(2)            | Null                 | No   | No   |
| **COUNTRY_CODE_3** | ISO 3 character country code.  e.g. USA. | CHAR(3)            | Null                 | No   | No   |
| **COUNTRY_NAME**   | ISO Country Name\.                       | VARCHAR2(100)      | Null                 | No   | No   |

[Back to index](./index.md)