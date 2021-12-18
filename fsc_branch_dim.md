# FSC_BRANCH_DIM

---

The location of the execution of a transaction.  e.g. Branch #123, ATM #3343433

| Attribute Name      | Attribute Definition                                                                   | Column Name         | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:--------------------|:---------------------------------------------------------------------------------------|:--------------------|:-------------------|:---------------------|:---------------|:---------------|
| branch_key          | Surrogate identifier..                                                                 | branch_key          | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id          | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id          | VARCHAR2(128)      | Not Null             | Yes            | No             |
| branch_type_desc    | "BRANCH" or "ATM" or "POS".  Used until Branch/ATM/Location are remodelled.            | branch_type_desc    | VARCHAR2(10)       | Null                 | No             | No             |
| branch_number       | Source System identifier for branches.                                                 | branch_number       | VARCHAR2(40)       | Null                 | No             | No             |
| branch_name         | Branch Name.                                                                           | branch_name         | VARCHAR2(100)      | Null                 | No             | No             |
| street_address_1    | Physical Address - Line 1.                                                             | street_address_1    | VARCHAR2(35)       | Null                 | No             | No             |
| street_address_2    | Physical Address - Line 2.                                                             | street_address_2    | VARCHAR2(35)       | Null                 | No             | No             |
| street_city_name    | Physical Address - City.                                                               | street_city_name    | VARCHAR2(35)       | Null                 | No             | No             |
| street_state_code   | Address State.                                                                         | street_state_code   | CHAR(3)            | Null                 | No             | No             |
| street_state_name   | State/Province etc name..                                                              | street_state_name   | VARCHAR2(35)       | Null                 | No             | No             |
| street_postal_code  | Address - Postal Code.                                                                 | street_postal_code  | CHAR(10)           | Null                 | No             | No             |
| street_country_code | Address - Country Code                                                                 | street_country_code | CHAR(3)            | Null                 | No             | No             |
| street_country_name | Address - Country Name                                                                 | street_country_name | VARCHAR2(100)      | Null                 | No             | No             |
| change_begin_date   | Date from which this row was valid..                                                   | change_begin_date   | DATE               | Null                 | No             | No             |
| change_end_date     | Date to which this row was valid..                                                     | change_end_date     | DATE               | Not Null             | No             | No             |
| change_current_ind  | Is this the current instance (Y/N).                                                    | change_current_ind  | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)