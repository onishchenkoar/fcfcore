# FSC_ASSOCIATE_DIM

---

An associate of the financial institution who has played a role in the execution of a transaction or plays a role in the managment of an account.  e.g. Teller, Insurance Agent, Account Manager.

[Back to index](./index.md)

| Column Name           | Column Definition                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:---------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| associate_key         | System generated surrogate identifier                                                  | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id            | Multibank configurations use this column to indicate which bank the record belongs to. | VARCHAR2(128)      | Not Null             | Yes  | No   |
| associate_number      | Firm-assigned associate identifier/employee number.                                    | VARCHAR2(20)       | Null                 | No   | No   |
| associate_first_name  | Associate First Name                                                                   | VARCHAR2(50)       | Null                 | No   | No   |
| associate_last_name   | Associate Last Name                                                                    | VARCHAR2(50)       | Null                 | No   | No   |
| associate_middle_name | Associate Middle Name                                                                  | VARCHAR2(100)      | Null                 | No   | No   |
| associate_title_desc  | Associate Title Sample data had a 39 char length.  Made it 50.                         | VARCHAR2(50)       | Null                 | No   | No   |
| associate_status_desc | Active, Terminated etc?                                                                | VARCHAR2(35)       | Null                 | No   | No   |
| street_address_1      | Associate's Address Line 1                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_address_2      | Associate's Address Line 2                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_city_name      | Associate's Address - City                                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_state_code     | Associate's Address - State Code                                                       | CHAR(3)            | Null                 | No   | No   |
| street_state_name     | Associate's Address - State/Province Name.                                             | VARCHAR2(35)       | Null                 | No   | No   |
| street_postal_code    | Associate's Address - Postal Code                                                      | CHAR(10)           | Null                 | No   | No   |
| street_country_name   | Associate's Address - Country (ISO)                                                    | VARCHAR2(100)      | Null                 | No   | No   |
| street_country_code   | Associate's Address - Country (ISO)                                                    | CHAR(3)            | Null                 | No   | No   |
| work_phone_number     | (XXX) XXX - XXXX                                                                       | VARCHAR2(25)       | Null                 | No   | No   |
| email_address         | XXXXXXXX@abc.com                                                                       | VARCHAR2(35)       | Null                 | No   | No   |
| branch_number         | Associate's branch number - if associated with a specific branch e.g. a teller.        | VARCHAR2(25)       | Null                 | No   | No   |
| branch_name           | Associate's branch name.                                                               | VARCHAR2(35)       | Null                 | No   | No   |
| change_begin_date     | Date from which this row was valid..                                                   | DATE               | Null                 | No   | No   |
| change_end_date       | Date to which this row was valid..                                                     | DATE               | Not Null             | No   | No   |
| change_current_ind    | Is this the current instance (Y/N).                                                    | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)