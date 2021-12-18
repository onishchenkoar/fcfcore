# FSC_PARTY_PROFILE_FACT

---

A monthly snapshot of a party's transactional activity.

| Attribute Name            | Attribute Definition                                                                                             | Column Name               | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:--------------------------|:-----------------------------------------------------------------------------------------------------------------|:--------------------------|:-------------------|:---------------------|:---------------|:---------------|
| party_number              | Source system's customer identifier..                                                                            | party_number              | VARCHAR2(50)       | Not Null             | Yes            | No             |
| month_key                 | Meaningful surrogate key of format yyyymm.                                                                       | month_key                 | NUMBER(6,0)        | Not Null             | No             | Yes            |
| segment_id                | Multibank configurations use this column to indicate which bank the record belongs to.                           | segment_id                | VARCHAR2(128)      | Not Null             | No             | Yes            |
| aggregate_assets_amount   | Total assets across all accounts.  Only includes assets, does not include loan amounts.                          | aggregate_assets_amount   | NUMBER(18,5)       | Null                 | No             | No             |
| total_wire_credits_amount | Total Wire Credits ($) to all accounts for the party during the period.                                          | total_wire_credits_amount | NUMBER(18,5)       | Null                 | No             | No             |
| total_wire_debits_amount  | Total Wire debits ($) to all accounts for the party during the period.                                           | total_wire_debits_amount  | NUMBER(18,5)       | Null                 | No             | No             |
| transactions_count        | Total number of transactions of accounts associated with this party during the profile period.                   | transactions_count        | NUMBER(10,0)       | Null                 | No             | No             |
| deposits_count            | Total number of deposits to accounts associated with this party during the profile period.                       | deposits_count            | NUMBER(10,0)       | Null                 | No             | No             |
| withdrawals_count         | Total number of withdrawls from accounts associated with this party during the profile period.                   | withdrawals_count         | NUMBER(10,0)       | Null                 | No             | No             |
| wires_count               | Total number of wires on accounts associated with this party during the profile period.                          | wires_count               | NUMBER(10,0)       | Null                 | No             | No             |
| cash_transactions_count   | Total number of cash transaction during the profile period.                                                      | cash_transactions_count   | NUMBER(10,0)       | Null                 | No             | No             |
| account_value_amount      | Total market value of accounts associated with this party at the end of the profile period.                      | account_value_amount      | NUMBER(18,5)       | Null                 | No             | No             |
| total_transactions_amount | Total money amount of all transactions (add up all debits and credits) for accounts associated with this party.  | total_transactions_amount | NUMBER(18,5)       | Null                 | No             | No             |
| total_credits_amount      | Total money amount of all credits for accounts associated with this party.                                       | total_credits_amount      | NUMBER(18,5)       | Null                 | No             | No             |
| total_debits_amount       | Total money amount of all debits for accounts associated with this party.                                        | total_debits_amount       | NUMBER(18,5)       | Null                 | No             | No             |
| total_cash_debits_amount  | Total money amount of all cash debits for accounts associated with this party.                                   | total_cash_debits_amount  | NUMBER(18,5)       | Null                 | No             | No             |
| total_cash_credits_amount | Total money amount of all cash credits for accounts associated with this party.                                  | total_cash_credits_amount | NUMBER(18,5)       | Null                 | No             | No             |
| largest_credit_amount     | Largest credit to any account associated with this party during the profile period.                              | largest_credit_amount     | NUMBER(18,5)       | Null                 | No             | No             |
| largest_debit_amount      | Largest debit to any account associated with this party during the profile period.                               | largest_debit_amount      | NUMBER(18,5)       | Null                 | No             | No             |
| funds_payment_svcs_count  | number of funds payment services to any account associated with this party during the profile period.            | funds_payment_svcs_count  | NUMBER(10,0)       | Null                 | No             | No             |
| funds_transfer_count      | Number of transfers to all accounts associated with this party during the profile period.                        | funds_transfer_count      | NUMBER(10)         | Null                 | No             | No             |
| monetary_instrument_count | Number of monetary instrument transactions on all accounts associated with this party during the profile period. | monetary_instrument_count | NUMBER(10)         | Null                 | No             | No             |

[Back to index](./README.md)