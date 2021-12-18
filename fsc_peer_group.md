# FSC_PEER_GROUP

---

Table to hold peer groups

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **PEER_GROUP_KEY**     | The surrogate key for the peer group.                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **PEER_GROUP_ID**      | The natural key for the peer group                                                     | VARCHAR2(50)       | Null                 | No   | No   |
| **PEER_GROUP_NAME**    | Peer group name                                                                        | VARCHAR2(50)       | Null                 | No   | No   |
| **PEER_GROUP_DESC**    | Peer group description                                                                 | VARCHAR2(200)      | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**  | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND** | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)