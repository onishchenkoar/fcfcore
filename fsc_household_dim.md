# FSC_HOUSEHOLD_DIM

---

Any grouping of parties or accounts which is considered relevant for anti-money laundering purposes.  The naming of this table suggest the traditional marketing definition of a household, but any grouping can be created.  The household type will describe the nature of the relationship.  A party can be in multiple households, but only one of a given type.

[Back to index](./index.md)

| Column Name                | Column Definition                                                                              | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:-----------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **HOUSEHOLD_KEY**          | System generated surrogate identifier\.                                                        | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**             | Multibank configurations use this column to indicate which bank the record belongs to.         | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **HOUSEHOLD_NUMBER**       | Source system identifier (if available).                                                       | VARCHAR2(50)       | Null                 | No   | No   |
| **HOUSEHOLD_TYPE_DESC**    | Client-specified household categorization.  e.g. "Common Address", "Common Phone", "Marketing" | VARCHAR2(20)       | Null                 | No   | No   |
| **STREET_ADDRESS_1**       | Household Physical Address - Line 1.                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_ADDRESS_2**       | Household Physical Address - Line 2.                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_CITY_NAME**       | Household Physical Address - City.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_STATE_CODE**      | Household Physical Address - State.                                                            | CHAR(3)            | Null                 | No   | No   |
| **STREET_STATE_NAME**      | Household Physical Address - State/Province etc name\.                                         | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_POSTAL_CODE**     | Household Physical Address - Postal Code.                                                      | VARCHAR(10)        | Null                 | No   | No   |
| **STREET_COUNTRY_CODE**    | Household Physical Address - Country Code (ISO).                                               | CHAR(3)            | Null                 | No   | No   |
| **STREET_COUNTRY_NAME**    | Street Country - Name (ISO).                                                                   | VARCHAR2(100)      | Null                 | No   | No   |
| **PHONE_NUMBER_1**         | Phone 1 (home?).                                                                               | VARCHAR2(25)       | Null                 | No   | No   |
| **PHONE_NUMBER_2**         | Phone 2(business?).                                                                            | VARCHAR2(25)       | Null                 | No   | No   |
| **HEAD_OF_HOUSEHOLD_NAME** | Name of head of household\.                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| **EMPLOYEE_IND**           | Is the party also an employee of the firm? Y/N.                                                | CHAR(1)            | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**      | Date from which this row was valid\.                                                           | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**        | Date to which this row was valid\.                                                             | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**     | Is this the current instance (Y/N).                                                            | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)