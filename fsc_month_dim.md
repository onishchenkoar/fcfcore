# **FSC_MONTH_DIM**

---

Calendar month table.

[Back to index](./index.md)

| Column Name       | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| month_key         | Meaningful surrogate key of format yyyymm.                                             | NUMBER(6,0)        | Not Null             | Yes  | No   |
| segment_id        | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| month_and_year    | Combined month and year e.g. 032003 (March 2003)                                       | CHAR(6)            | Null                 | No   | No   |
| month_name        | e.g. March                                                                             | VARCHAR2(9)        | Null                 | No   | No   |
| month_name_3c     | e.g. MAR                                                                               | CHAR(3)            | Null                 | No   | No   |
| quarter_name_2c   | e.g. Q1                                                                                | CHAR(2)            | Null                 | No   | No   |
| quarter_name_4c   | e.g. QTR1                                                                              | CHAR(4)            | Null                 | No   | No   |
| year_2c           | e.g. 03                                                                                | CHAR(2)            | Null                 | No   | No   |
| year_4c           | e.g. 2003                                                                              | CHAR(4)            | Null                 | No   | No   |
| current_month_ind | Is this the current month Y/N.                                                         | CHAR(1)            | Null                 | No   | No   |

[Back to index](./index.md)