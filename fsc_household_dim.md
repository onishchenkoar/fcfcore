# FSC_HOUSEHOLD_DIM

---

Any grouping of parties or accounts which is considered relevant for anti-money laundering purposes.  The naming of this table suggest the traditional marketing definition of a household, but any grouping can be created.  The household type will describe the nature of the relationship.  A party can be in multiple households, but only one of a given type.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                              | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:-----------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| household_key          | System generated surrogate identifier..                                                        | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id             | Multibank configurations use this column to indicate which bank the record belongs to.         | VARCHAR2(128)      | Not Null             | Yes  | No   |
| household_number       | Source system identifier (if available).                                                       | VARCHAR2(50)       | Null                 | No   | No   |
| household_type_desc    | Client-specified household categorization.  e.g. "Common Address", "Common Phone", "Marketing" | VARCHAR2(20)       | Null                 | No   | No   |
| street_address_1       | Household Physical Address - Line 1.                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| street_address_2       | Household Physical Address - Line 2.                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| street_city_name       | Household Physical Address - City.                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_state_code      | Household Physical Address - State.                                                            | CHAR(3)            | Null                 | No   | No   |
| street_state_name      | Household Physical Address - State/Province etc name..                                         | VARCHAR2(35)       | Null                 | No   | No   |
| street_postal_code     | Household Physical Address - Postal Code.                                                      | VARCHAR(10)        | Null                 | No   | No   |
| street_country_code    | Household Physical Address - Country Code (ISO).                                               | CHAR(3)            | Null                 | No   | No   |
| street_country_name    | Street Country - Name (ISO).                                                                   | VARCHAR2(100)      | Null                 | No   | No   |
| phone_number_1         | Phone 1 (home?).                                                                               | VARCHAR2(25)       | Null                 | No   | No   |
| phone_number_2         | Phone 2(business?).                                                                            | VARCHAR2(25)       | Null                 | No   | No   |
| head_of_household_name | Name of head of household..                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| employee_ind           | Is the party also an employee of the firm? Y/N.                                                | CHAR(1)            | Null                 | No   | No   |
| change_begin_date      | Date from which this row was valid..                                                           | DATE               | Null                 | No   | No   |
| change_end_date        | Date to which this row was valid..                                                             | DATE               | Not Null             | No   | No   |
| change_current_ind     | Is this the current instance (Y/N).                                                            | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)