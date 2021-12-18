# FSC_LOOKUP_DIM

---

Generic lookup table for storing values.

| Attribute Name           | Attribute Definition                                                                   | Column Name              | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------------|:-------------------|:---------------------|:---------------|:---------------|
| change_begin_date        | First date record is effective.                                                        | change_begin_date        | DATE               | Not Null             | No             | No             |
| change_current_ind       | Y or N flag indicating whether or not this is the current record.                      | change_current_ind       | CHAR(1)            | Not Null             | No             | No             |
| change_end_date          | Last date record is effective.                                                         | change_end_date          | DATE               | Not Null             | No             | No             |
| lookup_char_value        | Character value for lookup.                                                            | lookup_char_value        | VARCHAR2(50)       | Null                 | No             | No             |
| lookup_code              | The lookup code.                                                                       | lookup_code              | VARCHAR2(35)       | Not Null             | No             | No             |
| lookup_key               | Surrogate key for the lookup dimension.                                                | lookup_key               | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id               | VARCHAR2(128)      | Not Null             | Yes            | No             |
| lookup_level_1_type_code | Th level one look up type code.                                                        | lookup_level_1_type_code | VARCHAR2(3)        | Not Null             | No             | No             |
| lookup_level_2_type_code | The level two lookup type code.                                                        | lookup_level_2_type_code | VARCHAR2(28)       | Not Null             | No             | No             |
| lookup_num_value         | Numeric value for lookup.                                                              | lookup_num_value         | NUMBER(18,5)       | Null                 | No             | No             |
| lookup_date_value        | Date value for lookup.                                                                 | lookup_date_value        | DATE               | Null                 | No             | No             |

[Back to index](./README.md)