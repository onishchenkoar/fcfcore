# FSC_BRANCH_DIM

---

The location of the execution of a transaction.  e.g. Branch #123, ATM #3343433

[Back to index](./index.md)

| Column Name         | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| branch_key          | Surrogate identifier\.                                                                 | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| branch_type_desc    | "BRANCH" or "ATM" or "POS".  Used until Branch/ATM/Location are remodelled.            | VARCHAR2(10)       | Null                 | No   | No   |
| branch_number       | Source System identifier for branches.                                                 | VARCHAR2(40)       | Null                 | No   | No   |
| branch_name         | Branch Name.                                                                           | VARCHAR2(100)      | Null                 | No   | No   |
| street_address_1    | Physical Address - Line 1.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_address_2    | Physical Address - Line 2.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_city_name    | Physical Address - City.                                                               | VARCHAR2(35)       | Null                 | No   | No   |
| street_state_code   | Address State.                                                                         | CHAR(3)            | Null                 | No   | No   |
| street_state_name   | State/Province etc name\.                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| street_postal_code  | Address - Postal Code.                                                                 | CHAR(10)           | Null                 | No   | No   |
| street_country_code | Address - Country Code                                                                 | CHAR(3)            | Null                 | No   | No   |
| street_country_name | Address - Country Name                                                                 | VARCHAR2(100)      | Null                 | No   | No   |
| change_begin_date   | Date from which this row was valid\.                                                   | DATE               | Null                 | No   | No   |
| change_end_date     | Date to which this row was valid\.                                                     | DATE               | Not Null             | No   | No   |
| change_current_ind  | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)