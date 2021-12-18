# FSC_BRANCH_DIM

---

The location of the execution of a transaction.  e.g. Branch #123, ATM #3343433

[Back to index](./index.md)

| Column Name             | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **BRANCH_KEY**          | Surrogate identifier\.                                                                 | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**          | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **BRANCH_TYPE_DESC**    | "BRANCH" or "ATM" or "POS".  Used until Branch/ATM/Location are remodelled.            | VARCHAR2(10)       | Null                 | No   | No   |
| **BRANCH_NUMBER**       | Source System identifier for branches.                                                 | VARCHAR2(40)       | Null                 | No   | No   |
| **BRANCH_NAME**         | Branch Name.                                                                           | VARCHAR2(100)      | Null                 | No   | No   |
| **STREET_ADDRESS_1**    | Physical Address - Line 1.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_ADDRESS_2**    | Physical Address - Line 2.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_CITY_NAME**    | Physical Address - City.                                                               | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_STATE_CODE**   | Address State.                                                                         | CHAR(3)            | Null                 | No   | No   |
| **STREET_STATE_NAME**   | State/Province etc name\.                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_POSTAL_CODE**  | Address - Postal Code.                                                                 | CHAR(10)           | Null                 | No   | No   |
| **STREET_COUNTRY_CODE** | Address - Country Code                                                                 | CHAR(3)            | Null                 | No   | No   |
| **STREET_COUNTRY_NAME** | Address - Country Name                                                                 | VARCHAR2(100)      | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**   | Date from which this row was valid\.                                                   | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**     | Date to which this row was valid\.                                                     | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**  | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)