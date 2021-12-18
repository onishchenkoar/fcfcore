# FSC_CLASSIFIER_FACT

---

A monthly snapshot of a the risk classification factors for a customer. Stores intermediate data used by Risk Classification to produce Risk Assessments. This table will contain one record for each party for a given month_key.

[Back to index](./index.md)

| Column Name                   | Column Definition                                                                                                                                          | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| month_key                     | Meaningful surrogate key of format yyyymm.                                                                                                                 | NUMBER(6,0)        | Not Null             | No   | Yes  |
| party_number                  | Stores intermediate data used by Risk Classification to produce Risk Assessments. This table will contain one record for each party for a given month_key. | VARCHAR2(50)       | Not Null             | Yes  | No   |
| segment_id                    | Multibank configurations use this column to indicate which bank the record belongs to.                                                                     | VARCHAR2(128)      | Not Null             | No   | Yes  |
| rc_pep                        | Classifier based on politically_exposed_person_ind column in fsc_party_dim.                                                                                | NUMBER(1)          | Null                 | No   | No   |
| rc_professional_svcs_provider | Classifier based on partys status as a Professional Service Provider (e.g. attorney, CPA)                                                                  | NUMBER(1)          | Null                 | No   | No   |
| rc_deposit_broker             | Classifer based on whether or not the customer is a deposit broker.                                                                                        | NUMBER(1)          | Null                 | No   | No   |
| rc_foreign_financial_inst     | Classifer based on whether or not the customer is a foreign financial institution.                                                                         | NUMBER(1)          | Null                 | No   | No   |
| rc_non_bank_financial_inst    | Classifer based on whether or not the customer is a non bank financial institution.                                                                        | NUMBER(1)          | Null                 | No   | No   |
| rc_foreign_corporation        | Classifer based on whether or not the customer is a foreign corporation.                                                                                   | NUMBER(1)          | Null                 | No   | No   |
| rc_cash_intensive_business    | Classifer based on whether or not the customer is a cash intensive business.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| rc_private_banking            | Classifer based on whether or not the customer engaged in private banking.                                                                                 | NUMBER(1)          | Null                 | No   | No   |
| rc_trust_or_asset_mgmt_acct   | Classifer based on whether or not the customer has a trust or asset management account.                                                                    | NUMBER(1)          | Null                 | No   | No   |
| rc_foreign_correspondent_acct | Classifer based on whether or not the customer is a foreign correspondent account.                                                                         | NUMBER(1)          | Null                 | No   | No   |
| rc_trade_finance              | Classifer based on whether or not the customer is involved in trade finance.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| rc_special_use_account        | Classifer based on whether or not the customer is a special use account.                                                                                   | NUMBER(1)          | Null                 | No   | No   |
| rc_lending_activity           | Classifer based on whether or not the customer engaged in lending activity.                                                                                | NUMBER(1)          | Null                 | No   | No   |
| rc_nondeposit_account         | Classifer based on whether or not the customer is a nondeposit account.                                                                                    | NUMBER(1)          | Null                 | No   | No   |
| rc_wires_count                | Classifer based on number of wires in this period.                                                                                                         | NUMBER(6)          | Null                 | No   | No   |
| rc_funds_transfer_count       | Classifer based on the number of funds transfers in this period.                                                                                           | NUMBER(6)          | Null                 | No   | No   |
| rc_non_profit_org             | Classifer based on whether or not the customer is a non profit organization.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| rc_funds_payment_svcs_count   | Classifer based on number of funds payment services associated with the party in this month.                                                               | NUMBER(6)          | Null                 | No   | No   |
| rc_internal_pep               | Classifier based on a customer-supplied list of persons stored in fsk_list.                                                                                | NUMBER(1)          | Null                 | No   | No   |
| rc_high_risk_geography        | Classifer based on whether or not the customer is associated with a high risk geography.                                                                   | NUMBER(1)          | Null                 | No   | No   |
| rc_monetary_instrument_count  | Classifer based on number of monetary instruments associated with the party in this month.                                                                 | NUMBER(6)          | Null                 | No   | No   |

[Back to index](./index.md)