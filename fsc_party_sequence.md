# FSC_PARTY_SEQUENCE

---

The next identifier available to be used as a party_key in fsc_party_dim. This table is used by both the ETL process and the UI for generating new fsc_party_dim records. The user should read this value and immediately increment, update and commit to allow the next user access.

| Attribute Name   | Attribute Definition                                                                                                                                                                | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:---------------|:---------------|
| segment_id       | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                              | VARCHAR2(128)      | Not Null             | Yes            | No             |
| next_sequence_id | The next identifier available to be used as a party_key in fsc_party_dim. The user must read this value and immediately increment, update and commit to allow the next user access. | NUMBER(12)         | Not Null             | No             | No             |

[Back to index](./index.md)