# FSC_ENTITY_WATCH_LIST_DIM

---

External entities of interest for AML monitoring purposes obtained from publicly sourced lists.

[Back to index](./index.md)

| Column Name                        | Column Definition                                                                                                   | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------------|:--------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|| **ENTITY_WATCH_LIST_KEY**          | System generated surrogate key.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| **ENTITY_WATCH_LIST_NUMBER**       | Natural key for an individual list entry from source.  e.g. WorldCheck = UID.                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| **ENTITY_WATCH_LIST_NAME**         | Ten character code for watch list.                                                                                  | CHAR(10)           | Not Null             | No   | No   |
| **CATEGORY_DESC**                  | e.g. TERRORIST ORGANIZATION, PEP\.                                                                                  | VARCHAR2(50)       | Null                 | No   | No   |
| **TYPE_DESC**                      | Description of watch list type.                                                                                     | VARCHAR2(20)       | Null                 | No   | No   |
| **PROGRAMS**                       | Programs associated with this list (e.g. OFAC~ USDOJ~INTERPOL).                                                     | VARCHAR2(250)      | Null                 | No   | No   |
| **TAX_ID**                         | tax identification number - used as a means of unqiuely identifying an individual or organization. e.g. is USA SSN. | VARCHAR2(35)       | Null                 | No   | No   |
| **TAX_ID_TYPE_CODE**               | One letter code indicating type of tax id.                                                                          | CHAR(1)            | Null                 | No   | No   |
| **IDENTIFICATION_ID**              | identification id used to unqiuely identify an individual or organization.                                          | VARCHAR2(255)      | Null                 | No   | No   |
| **IDENTIFICATION_TYPE_DESC**       | Description of type of identification_id.                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| **DATE_OF_BIRTH**                  | Date of Birth.                                                                                                      | DATE               | Null                 | No   | No   |
| **YEAR_OF_BIRTH**                  | Year of Birth                                                                                                       | NUMBER(4)          | Null                 | No   | No   |
| **PLACE_OF_BIRTH**                 | Place of Birth                                                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| **DECEASED_IND**                   | Whether or not the subject is deceased. Y/N                                                                         | CHAR(1)            | Null                 | No   | No   |
| **FIRST_NAME**                     | First name of an individual.                                                                                        | VARCHAR2(350)      | Null                 | No   | No   |
| **LAST_NAME**                      | Last name of an individual                                                                                          | VARCHAR2(350)      | Null                 | No   | No   |
| **MIDDLE_NAME**                    | Middle name of an individual.                                                                                       | VARCHAR2(255)      | Null                 | No   | No   |
| **ENTITY_NAME**                    | Full name for individual or organization name                                                                       | VARCHAR2(800)      | Null                 | No   | No   |
| **MATCH_CODE_INDIVIDUAL**          | Match code constructed for individual names.                                                                        | VARCHAR2(200)      | Null                 | No   | No   |
| **MATCH_CODE_ORGANIZATION**        | Match code constructed for organization names.                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| **MATCH_CODE_ADDR_LINES**          | Match code constructed from street address. The match code represents address lines 1 and 2.                        | VARCHAR2(80)       | Null                 | No   | No   |
| **MATCH_CODE_CITY**                | Match code constructed from street address city name.                                                               | VARCHAR2(30)       | Null                 | No   | No   |
| **MATCH_CODE_STATE**               | Match code constructed from street address state or province name.                                                  | VARCHAR2(15)       | Null                 | No   | No   |
| **MATCH_CODE_COUNTRY**             | The country match code.                                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| **ENTITY_TITLE**                   | Title for entity (e.g. Mr., Mrs., Vice President, General)                                                          | VARCHAR2(200)      | Null                 | No   | No   |
| **OCCUPATION_DESC**                | Description of entity occupation.                                                                                   | VARCHAR2(500)      | Null                 | No   | No   |
| **ADDRESS**                        | Address                                                                                                             | VARCHAR2(750)      | Null                 | No   | No   |
| **CITY_NAME**                      | City Name                                                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| **STATE_NAME**                     | State Name                                                                                                          | VARCHAR2(50)       | Null                 | No   | No   |
| **POSTAL_CODE**                    | Postal Code                                                                                                         | CHAR(30)           | Null                 | No   | No   |
| **COUNTRY_CODE**                   | Country Code                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| **COUNTRY_NAME**                   | Country Name                                                                                                        | VARCHAR2(255)      | Null                 | No   | No   |
| **FULL_ADDRESS**                   | Full text of address                                                                                                | VARCHAR2(1200)     | Null                 | No   | No   |
| **MATCH_CODE_FULL_ADDRESS**        | Match code constructed from full address                                                                            | VARCHAR2(140)      | Null                 | No   | No   |
| **CITIZENSHIP_COUNTRY_CODE**       | Country of citizenship (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| **CITIZENSHIP_COUNTRY_NAME**       | Country of citizenship - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| **MATCH_CODE_CITIZENSHIP**         | Match code constructed from citizenship                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| **NATIONALITY_COUNTRY_CODE**       | Country of nationality (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| **NATIONALITY_COUNTRY_NAME**       | Country of nationality - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| **MATCH_CODE_NATIONALITY**         | Match code constructed from nationality                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| **ORG_COUNTRY_OF_BUSINESS_CODE**   | Country code for organization country of business                                                                   | VARCHAR2(3)        | Null                 | No   | No   |
| **ORG_COUNTRY_OF_BUSINESS_NAME**   | Country name for organization country of business                                                                   | VARCHAR2(100)      | Null                 | No   | No   |
| **MATCH_CODE_ORG_COUNTRY**         | Match code built from organization country name                                                                     | VARCHAR2(15)       | Null                 | No   | No   |
| **POLITICALLY_EXPOSED_PERSON_IND** | Is this person in a senior political position or related to a senior political person in some way? Y/N              | CHAR(1)            | Null                 | No   | No   |
| **TERROR**                         |                                                                                                                     | VARCHAR2(1 CHAR)   | Null                 | No   | No   |
| **ENTITY_TYPE**                    |                                                                                                                     | NUMBER(1,0)        | Null                 | No   | No   |
| **RESIDENT_ADRESS**                |                                                                                                                     | VARCHAR2(254 CHAR) | Null                 | No   | No   |
| **DIRECTOR**                       |                                                                                                                     | VARCHAR2(254 CHAR) | Null                 | No   | No   |
| **FOUNDER**                        |                                                                                                                     | VARCHAR2(254 CHAR) | Null                 | No   | No   |
| **ROW_ID**                         |                                                                                                                     | VARCHAR2(5 CHAR)   | Null                 | No   | No   |
| **TERRTYPE**                       |                                                                                                                     | VARCHAR2(254 CHAR) | Null                 | No   | No   |
| **CREATE_DATE**                    | date record was created                                                                                             | DATE               | Null                 | No   | No   |
| **UPDATE_DATE**                    | last update date for record                                                                                         | DATE               | Null                 | No   | No   |
| **EXCLUDE_IND**                    | Flag which user can set to exclude this entity from watch list analysis.                                            | CHAR(1)            | Not Null             | No   | No   |
| **CHANGE_BEGIN_DATE**              | First date this record is active                                                                                    | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**             | Flag indicating whether or not this is an active record.                                                            | CHAR(1)            | Not Null             | No   | No   |
| **CHANGE_END_DATE**                | Last date this record is active                                                                                     | DATE               | Not Null             | No   | No   |
| **PROCESSED_DTTM**                 |                                                                                                                     | DATE               | Not Null             | No   | No   |
| **PROCESSED_ID**                   |                                                                                                                     | NUMBER(8,0)        | Not Null             | No   | No   |
| **DATA_SOURCE**                    |                                                                                                                     | VARCHAR2(48 CHAR)  | Null                 | No   | No   |
| **ID_NUMBER**                      |                                                                                                                     | VARCHAR2(72 CHAR)  | Null                 | No   | No   |
| **STR_HASH**                       |                                                                                                                     | NUMBER             | Null                 | No   | No   |
| **LOCK_CHANGE_IND**                |                                                                                                                     | NUMBER             | Null                 | No   | No   |
| **TERROR_ID**                      |                                                                                                                     | VARCHAR2(10 CHAR)  | Null                 | No   | No   |
| **DECLINE_CODE**                   |                                                                                                                     | VARCHAR2(8 CHAR)   | Null                 | No   | No   |

[Back to index](./index.md)
