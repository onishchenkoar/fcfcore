# FSC_BANK_DIM

---

Describes a banking organization.  It may be an external bank or a unit of the client's organization.

| Attribute Name     | Attribute Definition                                                                   | Column Name        | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-------------------|:---------------------------------------------------------------------------------------|:-------------------|:-------------------|:---------------------|:---------------|:---------------|
| bank_key           | System generated surrogate identifier                                                  | bank_key           | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id         | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id         | VARCHAR2(128)      | Not Null             | Yes            | No             |
| bank_number        | Banks routing number e.g. ABA number                                                   | bank_number        | VARCHAR2(25)       | Null                 | No             | No             |
| bank_chips_number  | Banks number in CHIPS wire system                                                      | bank_chips_number  | VARCHAR2(25)       | Null                 | No             | No             |
| bank_swift_number  | Banks number in SWIFT wire system                                                      | bank_swift_number  | VARCHAR2(25)       | Null                 | No             | No             |
| bank_name          | Bank name                                                                              | bank_name          | VARCHAR2(35)       | Null                 | No             | No             |
| bank_address_1     | Bank Address Line 1                                                                    | bank_address_1     | VARCHAR2(35)       | Null                 | No             | No             |
| bank_address_2     | Bank Address Line 2                                                                    | bank_address_2     | VARCHAR2(35)       | Null                 | No             | No             |
| bank_city_name     | Bank City                                                                              | bank_city_name     | VARCHAR2(35)       | Null                 | No             | No             |
| bank_state_code    | Bank State                                                                             | bank_state_code    | CHAR(3)            | Null                 | No             | No             |
| bank_state_name    | Bank State/Province etc                                                                | bank_state_name    | VARCHAR2(35)       | Null                 | No             | No             |
| bank_postal_code   | Bank Postal Code                                                                       | bank_postal_code   | CHAR(10)           | Null                 | No             | No             |
| bank_country_code  | Bank country (ISO)                                                                     | bank_country_code  | CHAR(3)            | Null                 | No             | No             |
| bank_country_name  | This is really Bank Country Code (ISO) Should be a name and a code separately.         | bank_country_name  | CHAR(35)           | Null                 | No             | No             |
| bank_phone_number  | Bank Phone Number                                                                      | bank_phone_number  | VARCHAR2(25)       | Null                 | No             | No             |
| change_begin_date  | Date from which this row was valid.                                                    | change_begin_date  | DATE               | Null                 | No             | No             |
| change_end_date    | Date to which this row was valid.                                                      | change_end_date    | DATE               | Not Null             | No             | No             |
| change_current_ind | Is this the current instance (Y/N)                                                     | change_current_ind | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)