# FSC_BANK_DIM

---

Describes a banking organization.  It may be an external bank or a unit of the client's organization.

| Column Name        | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| bank_key           | System generated surrogate identifier                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| bank_number        | Banks routing number e.g. ABA number                                                   | VARCHAR2(25)       | Null                 | No   | No   |
| bank_chips_number  | Banks number in CHIPS wire system                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| bank_swift_number  | Banks number in SWIFT wire system                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| bank_name          | Bank name                                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| bank_address_1     | Bank Address Line 1                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| bank_address_2     | Bank Address Line 2                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| bank_city_name     | Bank City                                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| bank_state_code    | Bank State                                                                             | CHAR(3)            | Null                 | No   | No   |
| bank_state_name    | Bank State/Province etc                                                                | VARCHAR2(35)       | Null                 | No   | No   |
| bank_postal_code   | Bank Postal Code                                                                       | CHAR(10)           | Null                 | No   | No   |
| bank_country_code  | Bank country (ISO)                                                                     | CHAR(3)            | Null                 | No   | No   |
| bank_country_name  | This is really Bank Country Code (ISO) Should be a name and a code separately.         | CHAR(35)           | Null                 | No   | No   |
| bank_phone_number  | Bank Phone Number                                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| change_begin_date  | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| change_end_date    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| change_current_ind | Is this the current instance (Y/N)                                                     | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)