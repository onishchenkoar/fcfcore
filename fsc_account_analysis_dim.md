# FSC_ACCOUNT_ANALYSIS_DIM

---

Analytical data captured periodically (as often as client decides).  No history is maintained.

[Back to index](./index.md)

| Column Name                        | Column Definition                                                                                                                                                                                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ACCOUNT_NUMBER**                 | "Natural Key" from source system.  This may be concatenated e.g. division, branch, acct number\.                                                                                                                   | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**                     | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                             | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **EXPECTED_INCOMING_AMOUNT**       | Currency amount of credits expected to the account during the period (e.g. monthly).                                                                                                                               | NUMBER(18,5)       | Null                 | No   | No   |
| **EXPECTED_OUTGOING_AMOUNT**       | Currency amount of debits expected to the account during the period (e.g. monthly).                                                                                                                                | NUMBER(18,5)       | Null                 | No   | No   |
| **EXPECTED_INCOMING_COUNT**        | Number of credits expected to the account during the period (e.g. monthly).                                                                                                                                        | NUMBER(10)         | Null                 | No   | No   |
| **EXPECTED_OUTGOING_COUNT**        | Number of debits expected to the account during the period (e.g. monthly).                                                                                                                                         | NUMBER(10)         | Null                 | No   | No   |
| **INCREASED_BEHAVIOR_CREDIT_AMT**  | A threshold amount above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                                 | NUMBER(18,5)       | Null                 | No   | No   |
| **INCREASED_BEHAVIOR_DEBIT_AMT**   | A threshold amount above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                                 | NUMBER(18,5)       | Null                 | No   | No   |
| **INCREASED_BEHAVIOR_CREDIT_CNT**  | A threshold transaction count above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                      | NUMBER(15,5)       | Null                 | No   | No   |
| **INCREASED_BEHAVIOR_DEBIT_CNT**   | A threshold transaction count above which the behavior of the account is determined to have increased. See scenario SAS10088.                                                                                      | NUMBER(15,5)       | Null                 | No   | No   |
| **EXPECTED_CREDIT_CEILING_AMOUNT** | An expected total amount of credits to an account in a given period.  This is determined using the Largest Credit Amount field in the [Account Profile](./fsc_account_profile_fact.md).  Used in scenario SAS10091.                                 | NUMBER(18,5)       | Null                 | No   | No   |
| **EXPECTED_DEBIT_CEILING_AMOUNT**  | An expected total amount of debits to an account in a given period.  This is determined using the Largest Debit Amount field in the [Account Profile](./fsc_account_profile_fact.md).  Used in scenario SAS10091.                                   | NUMBER(18,5)       | Null                 | No   | No   |
| **LAST_ACTIVITY_DATE**             | Date the account last had activity.  Client determines if non-financial transactions should be included (e.g. inquiries), or whether bank-initiated transactions are included, and how often to update this field. | DATE               | Null                 | No   | No   |

[Back to index](./index.md)
