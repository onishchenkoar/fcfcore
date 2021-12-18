# FSC_PEER_GROUP_ENTITY_SUMMARY

---

table to hold entity summary statistics

[Back to index](./index.md)

| Column Name                  | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **SEGMENT_ID**               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **SUMMARY_PERIOD_CODE**      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| **SUMMARY_PERIOD_CODE**      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| **SUMMARY_PERIOD_CODE**      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| **SUMMARY_PERIOD_CODE**      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| **SUMMARY_DATE_KEY**         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| **SUMMARY_DATE_KEY**         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| **SUMMARY_DATE_KEY**         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| **SUMMARY_DATE_KEY**         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| **ENTITY_LEVEL_CODE**        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| **ENTITY_LEVEL_CODE**        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| **ENTITY_LEVEL_CODE**        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| **ENTITY_LEVEL_CODE**        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| **ENTITY_NUMBER**            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **ENTITY_NUMBER**            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **ENTITY_NUMBER**            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **ENTITY_NUMBER**            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **PROFILE_GROUP_ID**         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PROFILE_GROUP_ID**         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PROFILE_GROUP_ID**         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PROFILE_GROUP_ID**         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PROFILE_SUMMARY_ID**       | Summary group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **PROFILE_SUMMARY_ID**       | Summary group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| **SUMMARY_END_DATE_KEY**     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| **SUMMARY_END_DATE_KEY**     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| **TRANS_COUNT**              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| **TRANS_COUNT**              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| **TRANS_COUNT**              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| **TRANS_COUNT**              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| **TRANS_AMOUNT**             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TRANS_AMOUNT**             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TRANS_AMOUNT**             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **TRANS_AMOUNT**             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| **MAX_TRANS_AMOUNT**         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **MAX_TRANS_AMOUNT**         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **MAX_TRANS_AMOUNT**         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **MAX_TRANS_AMOUNT**         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| **ROUND_TRANS_AMOUNT**       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| **ROUND_TRANS_AMOUNT**       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| **ROUND_TRANS_AMOUNT**       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| **ROUND_TRANS_AMOUNT**       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| **NON_MONETARY_TRANS_COUNT** | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| **NON_MONETARY_TRANS_COUNT** | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| **NON_MONETARY_TRANS_COUNT** | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| **NON_MONETARY_TRANS_COUNT** | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| **LOG10TRANS_AMOUNT**        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10TRANS_AMOUNT**        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10TRANS_AMOUNT**        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10TRANS_AMOUNT**        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_MAX_TRANS_AMOUNT**   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_MAX_TRANS_AMOUNT**   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_MAX_TRANS_AMOUNT**   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_MAX_TRANS_AMOUNT**   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_COUNT**  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_COUNT**  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_COUNT**  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_COUNT**  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_AMOUNT** | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_AMOUNT** | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_AMOUNT** | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_ROUND_TRANS_AMOUNT** | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| **ROUND_TRANS_COUNT**        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| **ROUND_TRANS_COUNT**        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| **ROUND_TRANS_COUNT**        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| **ROUND_TRANS_COUNT**        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| **LOG10_TRANS_COUNT**        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_TRANS_COUNT**        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_TRANS_COUNT**        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| **LOG10_TRANS_COUNT**        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| **SUMMARY_END_DATE_KEY**     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| **SUMMARY_END_DATE_KEY**     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |

[Back to index](./index.md)