# FSC_PARTY_ASSOC

---

Relates one party to another. The relationship is described by the relationship_type_code.

[Back to index](./index.md)

| Column Name                | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PARTY_NUMBER**           | Source system's customer identifier\.                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PARTY_NUMBER**           | Source system's customer identifier\.                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **RELATIONSHIP_TYPE_CODE** | The type of relationship between the two parties.                                      | VARCHAR2(20)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **CHANGE_BEGIN_DATE**      | Date from which this row was valid.                                                    | DATE               | Not Null             | Yes  | No   |
| **CHANGE_END_DATE**        | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**     | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)