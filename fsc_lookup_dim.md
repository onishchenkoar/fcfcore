# FSC_LOOKUP_DIM

---

Generic lookup table for storing values.

[Back to index](./index.md)

| Column Name                  | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **CHANGE_BEGIN_DATE**        | First date record is effective.                                                        | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**       | Y or N flag indicating whether or not this is the current record.                      | CHAR(1)            | Not Null             | No   | No   |
| **CHANGE_END_DATE**          | Last date record is effective.                                                         | DATE               | Not Null             | No   | No   |
| **LOOKUP_CHAR_VALUE**        | Character value for lookup.                                                            | VARCHAR2(50)       | Null                 | No   | No   |
| **LOOKUP_CODE**              | The lookup code.                                                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| **LOOKUP_KEY**               | Surrogate key for the lookup dimension.                                                | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **LOOKUP_LEVEL_1_TYPE_CODE** | Th level one look up type code.                                                        | VARCHAR2(3)        | Not Null             | No   | No   |
| **LOOKUP_LEVEL_2_TYPE_CODE** | The level two lookup type code.                                                        | VARCHAR2(28)       | Not Null             | No   | No   |
| **LOOKUP_NUM_VALUE**         | Numeric value for lookup.                                                              | NUMBER(18,5)       | Null                 | No   | No   |
| **LOOKUP_DATE_VALUE**        | Date value for lookup.                                                                 | DATE               | Null                 | No   | No   |

[Back to index](./index.md)