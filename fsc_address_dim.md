# FSC_ADDRESS_DIM

---

Address table containing the additional addresses that cannot be stored in FSC_ACCOUT_DIM, FSC_HOUSEHOLD_DIM, and FSC_PARTY_DIM.

[Back to index](./index.md)

| Column Name               | Column Definition                                                                                                                                  | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **MATCH_CODE_CITY**       | Match code constructed from street address city name.                                                                                              | VARCHAR2(30)       | Null                 | No   | No   |
| **MATCH_CODE_COUNTRY**    | Match code constructed from street address country name.                                                                                           | VARCHAR2(15)       | Null                 | No   | No   |
| **MATCH_CODE_STATE**      | Match code constructed from street address state or province name                                                                                  | VARCHAR2(15)       | Null                 | No   | No   |
| **ADDRESS_KEY**           | Surrogate key for the address dimension.                                                                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| **SEGMENT_ID**            | Multibank configurations use this column to indicate which bank the record belongs to.                                                             | VARCHAR2(128)      | Not Null             | Yes  | No   |
| **ENTITY_TYPE**           | The entity type, for example PTY (party).                                                                                                          | CHAR(3)            | Null                 | No   | No   |
| **ADDRESS_LINE_1_TEXT**   | Physical Address - Line 1.                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| **ADDRESS_LINE_2_TEXT**   | Physical Address - Line 2.                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| **CITY_NAME**             | Physical Address - City.                                                                                                                           | VARCHAR2(35)       | Null                 | No   | No   |
| **STATE_CODE**            | Physical Address - State.                                                                                                                          | CHAR(3)            | Null                 | No   | No   |
| **STATE_NAME**            | State/Province etc name                                                                                                                            | VARCHAR2(35)       | Null                 | No   | No   |
| **POSTAL_CODE**           | Physical Address - Postal Code.                                                                                                                    | CHAR(10)           | Null                 | No   | No   |
| **COUNTRY_CODE**          | Physical Address - Country Code (ISO).                                                                                                             | CHAR(3)            | Null                 | No   | No   |
| **COUNTRY_NAME**          | Street Address - Country Name (ISO).                                                                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| **ADDRESS_TYPE_CODE**     | The address type code.                                                                                                                             | VARCHAR2(20)       | Null                 | No   | No   |
| **MATCH_CODE_ADDRESS**    | Match code address for individuals or organizations. Related Entities uses this field for comparisons. The match code represents the full address. | VARCHAR2(140)      | Null                 | No   | No   |
| **MATCH_CODE_ADDR_LINES** | Match code constructed from street address. The match code represents the address line 1 and address line 2.                                       | VARCHAR2(80)       | Null                 | No   | No   |
| **CHANGE_BEGIN_DATE**     | Date from which this row was valid.                                                                                                                | DATE               | Null                 | No   | No   |
| **CHANGE_END_DATE**       | Date to which this row was valid.                                                                                                                  | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**    | Is this the current instance (Y/N).                                                                                                                | CHAR(1)            | Not Null             | No   | No   |
| **PARTY_NUMBER**          | Source system's customer identifier\.                                                                                                              | VARCHAR2(50)       | Null                 | No   | Yes  |

[Back to index](./index.md)