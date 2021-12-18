# FSC_PARTY_ASSOC

---

Relates one party to another. The relationship is described by the relationship_type_code.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| party_number           | Source system's customer identifier..                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| party_number           | Source system's customer identifier..                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| relationship_type_code | The type of relationship between the two parties.                                      | VARCHAR2(20)       | Not Null             | Yes  | No   |
| segment_id             | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| change_begin_date      | Date from which this row was valid.                                                    | DATE               | Not Null             | Yes  | No   |
| change_end_date        | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| change_current_ind     | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)