# FSC_PARTY_ASSOC_ATTRIBUTE

---

table for defining the attributes for party to party relationship. For example, an record can be created to store the percentage of  John Doe owns ABC company where John Doe relates to ABC company as an Owner.

| Attribute Name         | Attribute Definition                                                                   | Column Name            | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-----------------------|:-------------------|:---------------------|:---------------|:---------------|
| party_number           | Source system's customer identifier..                                                  | party_number           | VARCHAR2(50)       | Not Null             | No             | Yes            |
| party_number           | Source system's customer identifier..                                                  | related_party_number   | VARCHAR2(50)       | Not Null             | No             | Yes            |
| relationship_type_code | The type of relationship between the two parties.                                      | relationship_type_code | VARCHAR2(20)       | Not Null             | No             | Yes            |
| attribute_type_code    | Party to party relationship attribute data type (CHAR, NUM, DATE)                      | attribute_type_code    | VARCHAR2(35)       | Not Null             | Yes            | No             |
| segment_id             | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id             | VARCHAR2(128)      | Not Null             | Yes            | No             |
| change_begin_date      | Date from which this row was valid.                                                    | change_begin_date      | DATE               | Not Null             | Yes            | No             |
| attribute_char_value   | The value of the party assoc attribute if it is a character value.                     | attribute_char_value   | VARCHAR2(32)       | Null                 | No             | No             |
| attribute_num_value    | The value of the party assoc attribute if it is a numeric value.                       | attribute_num_value    | NUMBER(18,5)       | Null                 | No             | No             |
| change_end_date        | Date to which this row was valid.                                                      | change_end_date        | DATE               | Not Null             | No             | No             |
| change_current_ind     | Is this the current instance (Y/N).                                                    | change_current_ind     | CHAR(1)            | Not Null             | No             | No             |
| attribute_date_value   | The value of the party assoc attribute if it is a date value.                          | attribute_date_value   | DATE               | Null                 | No             | No             |

[Back to index](./README.md)