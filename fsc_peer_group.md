# FSC_PEER_GROUP

---

Table to hold peer groups

| Attribute Name     | Attribute Definition                                                                   | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:---------------|:---------------|
| peer_group_key     | The surrogate key for the peer group.                                                  | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes            | No             |
| peer_group_id      | The natural key for the peer group                                                     | VARCHAR2(50)       | Null                 | No             | No             |
| peer_group_name    | Peer group name                                                                        | VARCHAR2(50)       | Null                 | No             | No             |
| peer_group_desc    | Peer group description                                                                 | VARCHAR2(200)      | Null                 | No             | No             |
| change_begin_date  | Date from which this row was valid.                                                    | DATE               | Null                 | No             | No             |
| change_end_date    | Date to which this row was valid.                                                      | DATE               | Not Null             | No             | No             |
| change_current_ind | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./index.md)