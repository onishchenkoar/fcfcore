# FSC_BANK_DIM

---

Describes a banking organization.  It may be an external bank or a unit of the client's organization.

[Back to index](./index.md)

| Column Name            | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **BANK_KEY**           | System generated surrogate identifier                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**         | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **BANK_NUMBER**        | Banks routing number e.g. ABA number                                                   | VARCHAR2(25)       | Null                 | No   | No   |
| **BANK_CHIPS_NUMBER**  | Banks number in CHIPS wire system                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| **BANK_SWIFT_NUMBER**  | Banks number in SWIFT wire system                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| **BANK_NAME**          | Bank name                                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| **BANK_ADDRESS_1**     | Bank Address Line 1                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| **BANK_ADDRESS_2**     | Bank Address Line 2                                                                    | VARCHAR2(35)       | Null                 | No   | No   |
| **BANK_CITY_NAME**     | Bank City                                                                              | VARCHAR2(35)       | Null                 | No   | No   |
| **BANK_STATE_CODE**    | Bank State                                                                             | CHAR(3)            | Null                 | No   | No   |
| **BANK_STATE_NAME**    | Bank State/Province etc                                                                | VARCHAR2(35)       | Null                 | No   | No   |
| **BANK_POSTAL_CODE**   | Bank Postal Code                                                                       | CHAR(10)           | Null                 | No   | No   |
| **BANK_COUNTRY_CODE**  | Bank country (ISO)                                                                     | CHAR(3)            | Null                 | No   | No   |
| **BANK_COUNTRY_NAME**  | This is really Bank Country Code (ISO) Should be a name and a code separately.         | CHAR(35)           | Null                 | No   | No   |
| **BANK_PHONE_NUMBER**  | Bank Phone Number                                                                      | VARCHAR2(25)       | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**  | Date from which this row was valid.                                                    | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**    | Date to which this row was valid.                                                      | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND** | Is this the current instance (Y/N)                                                     | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)