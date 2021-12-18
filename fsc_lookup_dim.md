# **FSC_LOOKUP_DIM**

---

Generic lookup table for storing values.

[Back to index](./index.md)

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| change_begin_date        | First date record is effective.                                                        | DATE               | Not Null             | No   | No   |
| change_current_ind       | Y or N flag indicating whether or not this is the current record.                      | CHAR(1)            | Not Null             | No   | No   |
| change_end_date          | Last date record is effective.                                                         | DATE               | Not Null             | No   | No   |
| lookup_char_value        | Character value for lookup.                                                            | VARCHAR2(50)       | Null                 | No   | No   |
| lookup_code              | The lookup code.                                                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| lookup_key               | Surrogate key for the lookup dimension.                                                | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| lookup_level_1_type_code | Th level one look up type code.                                                        | VARCHAR2(3)        | Not Null             | No   | No   |
| lookup_level_2_type_code | The level two lookup type code.                                                        | VARCHAR2(28)       | Not Null             | No   | No   |
| lookup_num_value         | Numeric value for lookup.                                                              | NUMBER(18,5)       | Null                 | No   | No   |
| lookup_date_value        | Date value for lookup.                                                                 | DATE               | Null                 | No   | No   |

[Back to index](./index.md)