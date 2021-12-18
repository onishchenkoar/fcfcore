# FSC_ASSOCIATE_DIM

---

An associate of the financial institution who has played a role in the execution of a transaction or plays a role in the managment of an account.  e.g. Teller, Insurance Agent, Account Manager.

| Attribute Name        | Attribute Definition                                                                   | Column Name           | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:----------------------|:---------------------------------------------------------------------------------------|:----------------------|:-------------------|:---------------------|:---------------|:---------------|
| associate_key         | System generated surrogate identifier                                                  | associate_key         | NUMBER(12)         | Not Null             | Yes            | No             |
| segment_id            | Multibank configurations use this column to indicate which bank the record belongs to. | segment_id            | VARCHAR2(128)      | Not Null             | Yes            | No             |
| associate_number      | Firm-assigned associate identifier/employee number.                                    | associate_number      | VARCHAR2(20)       | Null                 | No             | No             |
| associate_first_name  | Associate First Name                                                                   | associate_first_name  | VARCHAR2(50)       | Null                 | No             | No             |
| associate_last_name   | Associate Last Name                                                                    | associate_last_name   | VARCHAR2(50)       | Null                 | No             | No             |
| associate_middle_name | Associate Middle Name                                                                  | associate_middle_name | VARCHAR2(100)      | Null                 | No             | No             |
| associate_title_desc  | Associate Title Sample data had a 39 char length.  Made it 50.                         | associate_title_desc  | VARCHAR2(50)       | Null                 | No             | No             |
| associate_status_desc | Active, Terminated etc?                                                                | associate_status_desc | VARCHAR2(35)       | Null                 | No             | No             |
| street_address_1      | Associate's Address Line 1                                                             | street_address_1      | VARCHAR2(35)       | Null                 | No             | No             |
| street_address_2      | Associate's Address Line 2                                                             | street_address_2      | VARCHAR2(35)       | Null                 | No             | No             |
| street_city_name      | Associate's Address - City                                                             | street_city_name      | VARCHAR2(35)       | Null                 | No             | No             |
| street_state_code     | Associate's Address - State Code                                                       | street_state_code     | CHAR(3)            | Null                 | No             | No             |
| street_state_name     | Associate's Address - State/Province Name.                                             | street_state_name     | VARCHAR2(35)       | Null                 | No             | No             |
| street_postal_code    | Associate's Address - Postal Code                                                      | street_postal_code    | CHAR(10)           | Null                 | No             | No             |
| street_country_name   | Associate's Address - Country (ISO)                                                    | street_country_name   | VARCHAR2(100)      | Null                 | No             | No             |
| street_country_code   | Associate's Address - Country (ISO)                                                    | street_country_code   | CHAR(3)            | Null                 | No             | No             |
| work_phone_number     | (XXX) XXX - XXXX                                                                       | work_phone_number     | VARCHAR2(25)       | Null                 | No             | No             |
| email_address         | XXXXXXXX@abc.com                                                                       | email_address         | VARCHAR2(35)       | Null                 | No             | No             |
| branch_number         | Associate's branch number - if associated with a specific branch e.g. a teller.        | branch_number         | VARCHAR2(25)       | Null                 | No             | No             |
| branch_name           | Associate's branch name.                                                               | branch_name           | VARCHAR2(35)       | Null                 | No             | No             |
| change_begin_date     | Date from which this row was valid..                                                   | change_begin_date     | DATE               | Null                 | No             | No             |
| change_end_date       | Date to which this row was valid..                                                     | change_end_date       | DATE               | Not Null             | No             | No             |
| change_current_ind    | Is this the current instance (Y/N).                                                    | change_current_ind    | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)