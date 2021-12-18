# FSC_ADDRESS_DIM

[Back to index](./index.md)

---

Address table containing the additional addresses that cannot be stored in FSC_ACCOUT_DIM, FSC_HOUSEHOLD_DIM, and FSC_PARTY_DIM.

| Column Name           | Column Definition                                                                                                                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| match_code_city       | Match code constructed from street address city name.                                                                                              | VARCHAR2(30)       | Null                 | No   | No   |
| match_code_country    | Match code constructed from street address country name.                                                                                           | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_state      | Match code constructed from street address state or province name                                                                                  | VARCHAR2(15)       | Null                 | No   | No   |
| address_key           | Surrogate key for the address dimension.                                                                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id            | Multibank configurations use this column to indicate which bank the record belongs to.                                                             | VARCHAR2(128)      | Not Null             | Yes  | No   |
| entity_type           | The entity type, for example PTY (party).                                                                                                          | CHAR(3)            | Null                 | No   | No   |
| address_line_1_text   | Physical Address - Line 1.                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| address_line_2_text   | Physical Address - Line 2.                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| city_name             | Physical Address - City.                                                                                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| state_code            | Physical Address - State.                                                                                                                          | CHAR(3)            | Null                 | No   | No   |
| state_name            | State/Province etc name                                                                                                                            | VARCHAR2(35)       | Null                 | No   | No   |
| postal_code           | Physical Address - Postal Code.                                                                                                                    | CHAR(10)           | Null                 | No   | No   |
| country_code          | Physical Address - Country Code (ISO).                                                                                                             | CHAR(3)            | Null                 | No   | No   |
| country_name          | Street Address - Country Name (ISO).                                                                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| address_type_code     | The address type code.                                                                                                                             | VARCHAR2(20)       | Null                 | No   | No   |
| match_code_address    | Match code address for individuals or organizations. Related Entities uses this field for comparisons. The match code represents the full address. | VARCHAR2(140)      | Null                 | No   | No   |
| match_code_addr_lines | Match code constructed from street address. The match code represents the address line 1 and address line 2.                                       | VARCHAR2(80)       | Null                 | No   | No   |
| change_begin_date     | Date from which this row was valid.                                                                                                                | DATE               | Null                 | No   | No   |
| change_end_date       | Date to which this row was valid.                                                                                                                  | DATE               | Not Null             | No   | No   |
| change_current_ind    | Is this the current instance (Y/N).                                                                                                                | CHAR(1)            | Not Null             | No   | No   |
| party_number          | Source system's customer identifier..                                                                                                              | VARCHAR2(50)       | Null                 | No   | Yes  |

[Back to index](./index.md)