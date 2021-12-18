# FSC_PEER_GROUP_ENTITY_SUMMARY

[Back to index](./index.md)

---

table to hold entity summary statistics

| Column Name              | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| segment_id               | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| summary_period_code      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| summary_period_code      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| summary_period_code      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| summary_period_code      | Entity summary for D (Daily), W (Weekly), or M (Monthly) period.                       | CHAR(1)            | Not Null             | Yes  | No   |
| summary_date_key         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| summary_date_key         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| summary_date_key         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| summary_date_key         | The beginning of the peer group entity summary, for example: 20130125.                 | NUMBER(8)          | Not Null             | Yes  | No   |
| entity_level_code        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| entity_level_code        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| entity_level_code        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| entity_level_code        | ACC (account) or PTY (party)                                                           | CHAR(3)            | Not Null             | Yes  | No   |
| entity_number            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| entity_number            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| entity_number            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| entity_number            |                                                                                        | VARCHAR2(50)       | Not Null             | Yes  | No   |
| profile_group_id         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| profile_group_id         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| profile_group_id         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| profile_group_id         | Profile group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| profile_summary_id       | Summary group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| profile_summary_id       | Summary group identifier.                                                              | VARCHAR2(50)       | Not Null             | No   | Yes  |
| summary_end_date_key     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| summary_end_date_key     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| trans_count              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| trans_count              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| trans_count              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| trans_count              | Transaction count                                                                      | NUMBER(10)         | Null                 | No   | No   |
| trans_amount             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| trans_amount             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| trans_amount             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| trans_amount             | Transaction amount                                                                     | NUMBER(18,5)       | Null                 | No   | No   |
| max_trans_amount         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| max_trans_amount         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| max_trans_amount         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| max_trans_amount         | Maximum transaction amount                                                             | NUMBER(18,5)       | Null                 | No   | No   |
| round_trans_amount       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| round_trans_amount       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| round_trans_amount       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| round_trans_amount       | Total transaction amount for transactions in round amounts                             | NUMBER(18,5)       | Null                 | No   | No   |
| non_monetary_trans_count | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| non_monetary_trans_count | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| non_monetary_trans_count | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| non_monetary_trans_count | Non-monetary transaction count                                                         | NUMBER(10)         | Null                 | No   | No   |
| log10trans_amount        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10trans_amount        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10trans_amount        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10trans_amount        | log10 of the transaction amount                                                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10_max_trans_amount   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| log10_max_trans_amount   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| log10_max_trans_amount   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| log10_max_trans_amount   | log10 of the maximum transaction amount                                                | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_count  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_count  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_count  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_count  | log10 of the transaction amount of transactions in round amounts                       | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_amount | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_amount | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_amount | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| log10_round_trans_amount | log10 of the transaction count of transactions in round amounts                        | NUMBER(12,10)      | Null                 | No   | No   |
| round_trans_count        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| round_trans_count        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| round_trans_count        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| round_trans_count        | Count of transactions in round amounts                                                 | NUMBER(10)         | Null                 | No   | No   |
| log10_trans_count        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| log10_trans_count        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| log10_trans_count        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| log10_trans_count        | log10 of transaction count                                                             | NUMBER(12,10)      | Null                 | No   | No   |
| summary_end_date_key     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |
| summary_end_date_key     |                                                                                        | NUMBER(8)          | Not Null             | No   | No   |

[Back to index](./index.md)