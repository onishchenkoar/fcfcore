# FSC_PEER_GROUP

---

Table to hold peer groups

| Attribute Name     | Attribute Definition                                                                   | Column Name        | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:-------------------|:---------------------|:---------------|:---------------|
| peer_group_key     | The surrogate key for the peer group.                                                  | peer_group_key     | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id         | VARCHAR2(128)      | Not Null             | Yes            | No             |
| peer_group_id      | The natural key for the peer group                                                     | peer_group_id      | VARCHAR2(50)       | Null                 | No             | No             |
| peer_group_name    | Peer group name                                                                        | peer_group_name    | VARCHAR2(50)       | Null                 | No             | No             |
| peer_group_desc    | Peer group description                                                                 | peer_group_desc    | VARCHAR2(200)      | Null                 | No             | No             |
| change_begin_date  | Date from which this row was valid.                                                    | change_begin_date  | DATE               | Null                 | No             | No             |
| change_end_date    | Date to which this row was valid.                                                      | change_end_date    | DATE               | Not Null             | No             | No             |
| change_current_ind | Is this the current instance (Y/N).                                                    | change_current_ind | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)