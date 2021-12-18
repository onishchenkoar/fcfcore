# FSC_PARTY_ASSOC_ATTRIBUTE

---

table for defining the attributes for party to party relationship. For example, an record can be created to store the percentage of  John Doe owns ABC company where John Doe relates to ABC company as an Owner.

[Back to index](./index.md)

| Column Name                | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PARTY_NUMBER**           | Source system's customer identifier\.                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PARTY_NUMBER**           | Source system's customer identifier\.                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **RELATIONSHIP_TYPE_CODE** | The type of relationship between the two parties.                                      | VARCHAR2(20)       | Not Null             | No   | Yes  |
| **ATTRIBUTE_TYPE_CODE**    | Party to party relationship attribute data type (CHAR, NUM, DATE)                      | VARCHAR2(35)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CHANGE_BEGIN_DATE**      | Date from which this row was valid.                                                    | DATE               | Not Null             | Yes  | No   |
| **ATTRIBUTE_CHAR_VALUE**   | The value of the party assoc attribute if it is a character value.                     | VARCHAR2(32)       | Null                 | No   | No   |
| **ATTRIBUTE_NUM_VALUE**    | The value of the party assoc attribute if it is a numeric value.                       | NUMBER(18,5)       | Null                 | No   | No   |
| **CHANGE_END_DATE**        | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**     | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |
| **ATTRIBUTE_DATE_VALUE**   | The value of the party assoc attribute if it is a date value.                          | DATE               | Null                 | No   | No   |

[Back to index](./index.md)