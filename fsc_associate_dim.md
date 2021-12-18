# FSC_ASSOCIATE_DIM

---

An associate of the financial institution who has played a role in the execution of a transaction or plays a role in the managment of an account.  e.g. Teller, Insurance Agent, Account Manager.

[Back to index](./index.md)

| Column Name               | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **ASSOCIATE_KEY**         | System generated surrogate identifier                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **ASSOCIATE_NUMBER**      | Firm-assigned associate identifier/employee number.                                    | VARCHAR2(20)       | Null                 | No   | No   |
| **ASSOCIATE_FIRST_NAME**  | Associate First Name                                                                   | VARCHAR2(50)       | Null                 | No   | No   |
| **ASSOCIATE_LAST_NAME**   | Associate Last Name                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| **ASSOCIATE_MIDDLE_NAME** | Associate Middle Name                                                                  | VARCHAR2(100)      | Null                 | No   | No   |
| **ASSOCIATE_TITLE_DESC**  | Associate Title Sample data had a 39 char length.  Made it 50.                         | VARCHAR2(50)       | Null                 | No   | No   |
| **ASSOCIATE_STATUS_DESC** | Active, Terminated etc?                                                                | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_ADDRESS_1**      | Associate's Address Line 1                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_ADDRESS_2**      | Associate's Address Line 2                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_CITY_NAME**      | Associate's Address - City                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_STATE_CODE**     | Associate's Address - State Code                                                       | CHAR(3)            | Null                 | No   | No   |
| **STREET_STATE_NAME**     | Associate's Address - State/Province Name.                                             | VARCHAR2(35)       | Null                 | No   | No   |
| **STREET_POSTAL_CODE**    | Associate's Address - Postal Code                                                      | CHAR(10)           | Null                 | No   | No   |
| **STREET_COUNTRY_NAME**   | Associate's Address - Country (ISO)                                                    | VARCHAR2(100)      | Null                 | No   | No   |
| **STREET_COUNTRY_CODE**   | Associate's Address - Country (ISO)                                                    | CHAR(3)            | Null                 | No   | No   |
| **WORK_PHONE_NUMBER**     | (XXX) XXX - XXXX                                                                       | VARCHAR2(25)       | Null                 | No   | No   |
| **EMAIL_ADDRESS**         | XXXXXXXX@abc.com                                                                       | VARCHAR2(35)       | Null                 | No   | No   |
| **BRANCH_NUMBER**         | Associate's branch number - if associated with a specific branch e.g. a teller.        | VARCHAR2(25)       | Null                 | No   | No   |
| **BRANCH_NAME**           | Associate's branch name.                                                               | VARCHAR2(35)       | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**     | Date from which this row was valid\.                                                   | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**       | Date to which this row was valid\.                                                     | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**    | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)