# FSC_CLASSIFIER_FACT

---

A monthly snapshot of a the risk classification factors for a customer. Stores intermediate data used by Risk Classification to produce Risk Assessments. This table will contain one record for each party for a given month_key.

[Back to index](./index.md)

| Column Name                       | Column Definition                                                                                                                                          | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **MONTH_KEY**                     | Meaningful surrogate key of format yyyymm.                                                                                                                 | NUMBER(6,0)        | Not Null             | No   | Yes  |
| **PARTY_NUMBER**                  | Stores intermediate data used by Risk Classification to produce Risk Assessments. This table will contain one record for each party for a given MONTH_KEY. | VARCHAR2(50)       | Not Null             | Yes  | No   |
| **SEGMENT_ID**                    | Multibank configurations use this column to indicate which bank the record belongs to.                                                                     | VARCHAR2(128)      | Not Null             | No   | Yes  |
| **RC_PEP**                        | Classifier based on POLITICALLY_EXPOSED_PERSON_IND column in [FSC_PARTY_DIM](./fsc_party_dim.md).                                                                                | NUMBER(1)          | Null                 | No   | No   |
| **RC_PROFESSIONAL_SVCS_PROVIDER** | Classifier based on partys status as a Professional Service Provider (e.g. attorney, CPA)                                                                  | NUMBER(1)          | Null                 | No   | No   |
| **RC_DEPOSIT_BROKER**             | Classifer based on whether or not the customer is a deposit broker.                                                                                        | NUMBER(1)          | Null                 | No   | No   |
| **RC_FOREIGN_FINANCIAL_INST**     | Classifer based on whether or not the customer is a foreign financial institution.                                                                         | NUMBER(1)          | Null                 | No   | No   |
| **RC_NON_BANK_FINANCIAL_INST**    | Classifer based on whether or not the customer is a non bank financial institution.                                                                        | NUMBER(1)          | Null                 | No   | No   |
| **RC_FOREIGN_CORPORATION**        | Classifer based on whether or not the customer is a foreign corporation.                                                                                   | NUMBER(1)          | Null                 | No   | No   |
| **RC_CASH_INTENSIVE_BUSINESS**    | Classifer based on whether or not the customer is a cash intensive business.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| **RC_PRIVATE_BANKING**            | Classifer based on whether or not the customer engaged in private banking.                                                                                 | NUMBER(1)          | Null                 | No   | No   |
| **RC_TRUST_OR_ASSET_MGMT_ACCT**   | Classifer based on whether or not the customer has a trust or asset management account.                                                                    | NUMBER(1)          | Null                 | No   | No   |
| **RC_FOREIGN_CORRESPONDENT_ACCT** | Classifer based on whether or not the customer is a foreign correspondent account.                                                                         | NUMBER(1)          | Null                 | No   | No   |
| **RC_TRADE_FINANCE**              | Classifer based on whether or not the customer is involved in trade finance.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| **RC_SPECIAL_USE_ACCOUNT**        | Classifer based on whether or not the customer is a special use account.                                                                                   | NUMBER(1)          | Null                 | No   | No   |
| **RC_LENDING_ACTIVITY**           | Classifer based on whether or not the customer engaged in lending activity.                                                                                | NUMBER(1)          | Null                 | No   | No   |
| **RC_NONDEPOSIT_ACCOUNT**         | Classifer based on whether or not the customer is a nondeposit account.                                                                                    | NUMBER(1)          | Null                 | No   | No   |
| **RC_WIRES_COUNT**                | Classifer based on number of wires in this period.                                                                                                         | NUMBER(6)          | Null                 | No   | No   |
| **RC_FUNDS_TRANSFER_COUNT**       | Classifer based on the number of funds transfers in this period.                                                                                           | NUMBER(6)          | Null                 | No   | No   |
| **RC_NON_PROFIT_ORG**             | Classifer based on whether or not the customer is a non profit organization.                                                                               | NUMBER(1)          | Null                 | No   | No   |
| **RC_FUNDS_PAYMENT_SVCS_COUNT**   | Classifer based on number of funds payment services associated with the party in this month.                                                               | NUMBER(6)          | Null                 | No   | No   |
| **RC_INTERNAL_PEP**               | Classifier based on a customer-supplied list of persons stored in [FSK_LIST](https://onishchenkoar.github.io/fcfkc/fsk_list).                                                                                | NUMBER(1)          | Null                 | No   | No   |
| **RC_HIGH_RISK_GEOGRAPHY**        | Classifer based on whether or not the customer is associated with a high risk geography.                                                                   | NUMBER(1)          | Null                 | No   | No   |
| **RC_MONETARY_INSTRUMENT_COUNT**  | Classifer based on number of monetary instruments associated with the party in this month.                                                                 | NUMBER(6)          | Null                 | No   | No   |

[Back to index](./index.md)
