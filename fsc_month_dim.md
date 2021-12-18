# FSC_MONTH_DIM

---

Calendar month table.

[Back to index](./index.md)

| Column Name           | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **MONTH_KEY**         | Meaningful surrogate key of format yyyymm.                                             | NUMBER(6,0)        | Not Null             | Yes  | No   |
| **SEGMENT_ID**        | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **MONTH_AND_YEAR**    | Combined month and year e.g. 032003 (March 2003)                                       | CHAR(6)            | Null                 | No   | No   |
| **MONTH_NAME**        | e.g. March                                                                             | VARCHAR2(9)        | Null                 | No   | No   |
| **MONTH_NAME_3C**     | e.g. MAR                                                                               | CHAR(3)            | Null                 | No   | No   |
| **QUARTER_NAME_2C**   | e.g. Q1                                                                                | CHAR(2)            | Null                 | No   | No   |
| **QUARTER_NAME_4C**   | e.g. QTR1                                                                              | CHAR(4)            | Null                 | No   | No   |
| **YEAR_2C**           | e.g. 03                                                                                | CHAR(2)            | Null                 | No   | No   |
| **YEAR_4C**           | e.g. 2003                                                                              | CHAR(4)            | Null                 | No   | No   |
| **CURRENT_MONTH_IND** | Is this the current month Y/N.                                                         | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)