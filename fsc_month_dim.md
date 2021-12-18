# FSC_MONTH_DIM

---

Calendar month table.

| Attribute Name    | Attribute Definition                                                                   | Column Name       | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:------------------|:---------------------------------------------------------------------------------------|:------------------|:-------------------|:---------------------|:---------------|:---------------|
| month_key         | Meaningful surrogate key of format yyyymm.                                             | month_key         | NUMBER(6,0)        | Not Null             | Yes            | No             |
| segment_id        | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id        | VARCHAR2(128)      | Not Null             | Yes            | No             |
| month_and_year    | Combined month and year e.g. 032003 (March 2003)                                       | month_and_year    | CHAR(6)            | Null                 | No             | No             |
| month_name        | e.g. March                                                                             | month_name        | VARCHAR2(9)        | Null                 | No             | No             |
| month_name_3c     | e.g. MAR                                                                               | month_name_3c     | CHAR(3)            | Null                 | No             | No             |
| quarter_name_2c   | e.g. Q1                                                                                | quarter_name_2c   | CHAR(2)            | Null                 | No             | No             |
| quarter_name_4c   | e.g. QTR1                                                                              | quarter_name_4c   | CHAR(4)            | Null                 | No             | No             |
| year_2c           | e.g. 03                                                                                | year_2c           | CHAR(2)            | Null                 | No             | No             |
| year_4c           | e.g. 2003                                                                              | year_4c           | CHAR(4)            | Null                 | No             | No             |
| current_month_ind | Is this the current month Y/N.                                                         | current_month_ind | CHAR(1)            | Null                 | No             | No             |

[Back to index](./README.md)