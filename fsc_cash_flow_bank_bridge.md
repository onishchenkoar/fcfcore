# FSC_CASH_FLOW_BANK_BRIDGE

---

A record of which banks play a role on a given cash flow transaction.  Roles include REMITTER and BENEFICIARY.

| Attribute Name   | Attribute Definition                                                                                                                                                                                                                                    | Column Name     | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:-------------------|:---------------------|:---------------|:---------------|
| bank_key         | System generated surrogate identifier                                                                                                                                                                                                                   | bank_key        | NUMBER(12)         | Not Null             | No             | Yes            |
| transaction_key  | Surrogate key                                                                                                                                                                                                                                           | transaction_key | NUMBER(12)         | Not Null             | No             | Yes            |
| segment_id       | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                                                  | segment_id      | VARCHAR2(128)      | Not Null             | No             | Yes            |
| role_desc        | Role that the bank plays in the transaction. Starter Values are: BENEFICIARY REMITTER CORRESPONDENT INTERMEDIARY Note: Likely not possible to be able to differentiate between correspondent and intermediary - probably best to just use intermediary. | role_desc       | VARCHAR2(20)       | Null                 | No             | No             |
| sequence_number  | Order in which the bank handled the monies.                                                                                                                                                                                                             | sequence_number | NUMBER(2)          | Null                 | No             | No             |

[Back to index](./README.md)