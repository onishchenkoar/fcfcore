# FSC_PEER_GROUP_ASSIGNMENT

---

Table to hold which peer groups are assigned to entities

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ENTITY_LEVEL_CODE**  | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| **ENTITY_KEY**         | They key to the entity, which can be an account, party, etc?                           | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PEER_GROUP_KEY**     | The surrogate key for the peer group.                                                  | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **CHANGE_BEGIN_DATE**  | Date from which this row was valid.                                                    | DATE               | Not Null             | Yes  | No   |
| **CHANGE_END_DATE**    | Date to which this row was valid\.                                                     | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND** | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)