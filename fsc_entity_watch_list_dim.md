# **FSC_ENTITY_WATCH_LIST_DIM**

---

External entities of interest for AML monitoring purposes obtained from publicly sourced lists.

[Back to index](./index.md)

| Column Name                    | Column Definition                                                                                                   | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------------|:--------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| match_code_country             | The country match code.                                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_country             | The country match code.                                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| entity_watch_list_key          | System generated surrogate key.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| entity_watch_list_key          | System generated surrogate key.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| entity_watch_list_key          | System generated surrogate key.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| entity_watch_list_key          | System generated surrogate key.                                                                                     | NUMBER(12)         | Not Null             | Yes  | No   |
| entity_watch_list_number       | Natural key for an individual list entry from source.  e.g. WorldCheck = UID.                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| entity_watch_list_number       | Natural key for an individual list entry from source.  e.g. WorldCheck = UID.                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| entity_watch_list_number       | Natural key for an individual list entry from source.  e.g. WorldCheck = UID.                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| entity_watch_list_number       | Natural key for an individual list entry from source.  e.g. WorldCheck = UID.                                       | VARCHAR2(35)       | Not Null             | No   | No   |
| watch_list_name                | Four character code for watch list.                                                                                 | CHAR(4)            | Not Null             | No   | No   |
| watch_list_name                | Four character code for watch list.                                                                                 | CHAR(4)            | Not Null             | No   | No   |
| watch_list_name                | Four character code for watch list.                                                                                 | CHAR(4)            | Not Null             | No   | No   |
| watch_list_name                | Four character code for watch list.                                                                                 | CHAR(4)            | Not Null             | No   | No   |
| category_desc                  | e.g. TERRORIST ORGANIZATION, PEP\.                                                                                  | VARCHAR2(50)       | Null                 | No   | No   |
| category_desc                  | e.g. TERRORIST ORGANIZATION, PEP\.                                                                                  | VARCHAR2(50)       | Null                 | No   | No   |
| type_desc                      | Description of watch list type.                                                                                     | VARCHAR2(20)       | Null                 | No   | No   |
| type_desc                      | Description of watch list type.                                                                                     | VARCHAR2(20)       | Null                 | No   | No   |
| programs                       | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).                                                      | VARCHAR2(250)      | Null                 | No   | No   |
| programs                       | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).                                                      | VARCHAR2(250)      | Null                 | No   | No   |
| type_desc                      | Description of watch list type.                                                                                     | VARCHAR2(20)       | Null                 | No   | No   |
| type_desc                      | Description of watch list type.                                                                                     | VARCHAR2(20)       | Null                 | No   | No   |
| identification_id              | identification id used to unqiuely identify an individual or organization.                                          | VARCHAR2(255)      | Null                 | No   | No   |
| identification_id              | identification id used to unqiuely identify an individual or organization.                                          | VARCHAR2(255)      | Null                 | No   | No   |
| programs                       | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).                                                      | VARCHAR2(250)      | Null                 | No   | No   |
| programs                       | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).                                                      | VARCHAR2(250)      | Null                 | No   | No   |
| identification_type_desc       | Description of type of identification_id.                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| identification_type_desc       | Description of type of identification_id.                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| tax_id                         | tax identification number - used as a means of unqiuely identifying an individual or organization. e.g. is USA SSN. | VARCHAR2(35)       | Null                 | No   | No   |
| tax_id                         | tax identification number - used as a means of unqiuely identifying an individual or organization. e.g. is USA SSN. | VARCHAR2(35)       | Null                 | No   | No   |
| entity_name                    | Full name for individual or organization name                                                                       | VARCHAR2(800)      | Null                 | No   | No   |
| entity_name                    | Full name for individual or organization name                                                                       | VARCHAR2(800)      | Null                 | No   | No   |
| tax_id_type_code               | One letter code indicating type of tax id.                                                                          | CHAR(1)            | Null                 | No   | No   |
| tax_id_type_code               | One letter code indicating type of tax id.                                                                          | CHAR(1)            | Null                 | No   | No   |
| identification_id              | identification id used to unqiuely identify an individual or organization.                                          | VARCHAR2(255)      | Null                 | No   | No   |
| identification_id              | identification id used to unqiuely identify an individual or organization.                                          | VARCHAR2(255)      | Null                 | No   | No   |
| match_code_individual          | Match code constructed for individual names.                                                                        | VARCHAR2(200)      | Null                 | No   | No   |
| match_code_individual          | Match code constructed for individual names.                                                                        | VARCHAR2(200)      | Null                 | No   | No   |
| identification_type_desc       | Description of type of identification_id.                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| identification_type_desc       | Description of type of identification_id.                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| match_code_organization        | Match code constructed for organization names.                                                                      | VARCHAR2(200)      | Null                 | No   | No   |
| match_code_organization        | Match code constructed for organization names.                                                                      | VARCHAR2(200)      | Null                 | No   | No   |
| address                        | Address                                                                                                             | VARCHAR2(750)      | Null                 | No   | No   |
| address                        | Address                                                                                                             | VARCHAR2(750)      | Null                 | No   | No   |
| date_of_birth                  | Date of Birth.                                                                                                      | DATE               | Null                 | No   | No   |
| date_of_birth                  | Date of Birth.                                                                                                      | DATE               | Null                 | No   | No   |
| city_name                      | City Name                                                                                                           | VARCHAR2(155)      | Null                 | No   | No   |
| city_name                      | City Name                                                                                                           | VARCHAR2(155)      | Null                 | No   | No   |
| year_of_birth                  | Year of Birth                                                                                                       | NUMBER(4)          | Null                 | No   | No   |
| year_of_birth                  | Year of Birth                                                                                                       | NUMBER(4)          | Null                 | No   | No   |
| place_of_birth                 | Place of Birth                                                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| place_of_birth                 | Place of Birth                                                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| state_name                     | State Name                                                                                                          | VARCHAR2(50)       | Null                 | No   | No   |
| state_name                     | State Name                                                                                                          | VARCHAR2(50)       | Null                 | No   | No   |
| country_code                   | Country Code                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| country_code                   | Country Code                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| deceased_ind                   | Whether or not the subject is deceased. Y|N                                                                         | CHAR(1)            | Null                 | No   | No   |
| deceased_ind                   | Whether or not the subject is deceased. Y|N                                                                         | CHAR(1)            | Null                 | No   | No   |
| country_name                   | Country Name                                                                                                        | VARCHAR2(255)      | Null                 | No   | No   |
| country_name                   | Country Name                                                                                                        | VARCHAR2(255)      | Null                 | No   | No   |
| first_name                     | First name of an individual.                                                                                        | VARCHAR2(350)      | Null                 | No   | No   |
| first_name                     | First name of an individual.                                                                                        | VARCHAR2(350)      | Null                 | No   | No   |
| create_date                    | date record was created                                                                                             | DATE               | Null                 | No   | No   |
| create_date                    | date record was created                                                                                             | DATE               | Null                 | No   | No   |
| last_name                      | Last name of an individual                                                                                          | VARCHAR2(350)      | Null                 | No   | No   |
| last_name                      | Last name of an individual                                                                                          | VARCHAR2(350)      | Null                 | No   | No   |
| middle_name                    | Middle name of an individual.                                                                                       | VARCHAR2(255)      | Null                 | No   | No   |
| middle_name                    | Middle name of an individual.                                                                                       | VARCHAR2(255)      | Null                 | No   | No   |
| update_date                    | last update date for record                                                                                         | DATE               | Null                 | No   | No   |
| update_date                    | last update date for record                                                                                         | DATE               | Null                 | No   | No   |
| entity_name                    | Full name for individual or organization name                                                                       | VARCHAR2(800)      | Null                 | No   | No   |
| entity_name                    | Full name for individual or organization name                                                                       | VARCHAR2(800)      | Null                 | No   | No   |
| exclude_ind                    | Flag which user can set to exclude this entity from watch list analysis.                                            | CHAR(1)            | Not Null             | No   | No   |
| exclude_ind                    | Flag which user can set to exclude this entity from watch list analysis.                                            | CHAR(1)            | Not Null             | No   | No   |
| change_begin_date              | First date this record is active                                                                                    | DATE               | Not Null             | No   | No   |
| change_begin_date              | First date this record is active                                                                                    | DATE               | Not Null             | No   | No   |
| match_code_individual          | Match code constructed for individual names.                                                                        | VARCHAR2(80)       | Null                 | No   | No   |
| match_code_individual          | Match code constructed for individual names.                                                                        | VARCHAR2(80)       | Null                 | No   | No   |
| change_end_date                | Last date this record is active                                                                                     | DATE               | Not Null             | No   | No   |
| change_end_date                | Last date this record is active                                                                                     | DATE               | Not Null             | No   | No   |
| match_code_organization        | Match code constructed for organization names.                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| match_code_organization        | Match code constructed for organization names.                                                                      | VARCHAR2(100)      | Null                 | No   | No   |
| change_current_ind             | Flag indicating whether or not this is an active record.                                                            | CHAR(1)            | Not Null             | No   | No   |
| change_current_ind             | Flag indicating whether or not this is an active record.                                                            | CHAR(1)            | Not Null             | No   | No   |
| entity_title                   | Title for entity (e.g. Mr., Mrs., Vice President, General)                                                          | VARCHAR2(200)      | Null                 | No   | No   |
| entity_title                   | Title for entity (e.g. Mr., Mrs., Vice President, General)                                                          | VARCHAR2(200)      | Null                 | No   | No   |
| match_code_addr_lines          | Match code constructed from street address. The match code represents address lines 1 and 2.                        | VARCHAR2(200)      | Null                 | No   | No   |
| match_code_addr_lines          | Match code constructed from street address. The match code represents address lines 1 and 2.                        | VARCHAR2(200)      | Null                 | No   | No   |
| occupation_desc                | Description of entity occupation.                                                                                   | VARCHAR2(500)      | Null                 | No   | No   |
| occupation_desc                | Description of entity occupation.                                                                                   | VARCHAR2(500)      | Null                 | No   | No   |
| address                        | Address                                                                                                             | VARCHAR2(750)      | Null                 | No   | No   |
| address                        | Address                                                                                                             | VARCHAR2(750)      | Null                 | No   | No   |
| city_name                      | City Name                                                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| city_name                      | City Name                                                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| state_name                     | State Name                                                                                                          | VARCHAR2(50)       | Null                 | No   | No   |
| state_name                     | State Name                                                                                                          | VARCHAR2(50)       | Null                 | No   | No   |
| postal_code                    | Postal Code                                                                                                         | CHAR(30)           | Null                 | No   | No   |
| postal_code                    | Postal Code                                                                                                         | CHAR(30)           | Null                 | No   | No   |
| country_code                   | Country Code                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| country_code                   | Country Code                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| country_name                   | Country Name                                                                                                        | VARCHAR2(255)      | Null                 | No   | No   |
| country_name                   | Country Name                                                                                                        | VARCHAR2(255)      | Null                 | No   | No   |
| full_address                   | Full text of address                                                                                                | VARCHAR2(1200)     | Null                 | No   | No   |
| full_address                   | Full text of address                                                                                                | VARCHAR2(1200)     | Null                 | No   | No   |
| match_code_full_address        | Match code constructed from full address                                                                            | VARCHAR2(140)      | Null                 | No   | No   |
| match_code_full_address        | Match code constructed from full address                                                                            | VARCHAR2(140)      | Null                 | No   | No   |
| citizenship_country_code       | Country of citizenship (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| citizenship_country_code       | Country of citizenship (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| citizenship_country_name       | Country of citizenship - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| citizenship_country_name       | Country of citizenship - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| match_code_citizenship         | Match code constructed from citizenship                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_citizenship         | Match code constructed from citizenship                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| nationality_country_code       | Country of nationality (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| nationality_country_code       | Country of nationality (ISO-3) for individual.                                                                      | CHAR(3)            | Null                 | No   | No   |
| nationality_country_name       | Country of nationality - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| nationality_country_name       | Country of nationality - name - for individual (ISO).                                                               | VARCHAR2(100)      | Null                 | No   | No   |
| match_code_nationality         | Match code constructed from nationality                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_nationality         | Match code constructed from nationality                                                                             | VARCHAR2(15)       | Null                 | No   | No   |
| org_country_of_business_code   | Country code for organization country of business                                                                   | VARCHAR2(3)        | Null                 | No   | No   |
| org_country_of_business_code   | Country code for organization country of business                                                                   | VARCHAR2(3)        | Null                 | No   | No   |
| org_country_of_business_name   | Country name for organization country of business                                                                   | VARCHAR2(100)      | Null                 | No   | No   |
| org_country_of_business_name   | Country name for organization country of business                                                                   | VARCHAR2(100)      | Null                 | No   | No   |
| match_code_org_country         | Match code built from organization country name                                                                     | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_org_country         | Match code built from organization country name                                                                     | VARCHAR2(15)       | Null                 | No   | No   |
| politically_exposed_person_ind | Is this person in a senior political position or related to a senior political person in some way? Y/N              | CHAR(1)            | Null                 | No   | No   |
| politically_exposed_person_ind | Is this person in a senior political position or related to a senior political person in some way? Y/N              | CHAR(1)            | Null                 | No   | No   |
| create_date                    | date record was created                                                                                             | DATE               | Null                 | No   | No   |
| create_date                    | date record was created                                                                                             | DATE               | Null                 | No   | No   |
| update_date                    | last update date for record                                                                                         | DATE               | Null                 | No   | No   |
| update_date                    | last update date for record                                                                                         | DATE               | Null                 | No   | No   |
| exclude_ind                    | Flag which user can set to exclude this entity from watch list analysis.                                            | CHAR(1)            | Not Null             | No   | No   |
| exclude_ind                    | Flag which user can set to exclude this entity from watch list analysis.                                            | CHAR(1)            | Not Null             | No   | No   |
| change_begin_date              | First date this record is active                                                                                    | DATE               | Not Null             | No   | No   |
| change_begin_date              | First date this record is active                                                                                    | DATE               | Not Null             | No   | No   |
| change_end_date                | Last date this record is active                                                                                     | DATE               | Not Null             | No   | No   |
| change_end_date                | Last date this record is active                                                                                     | DATE               | Not Null             | No   | No   |
| change_current_ind             | Flag indicating whether or not this is an active record.                                                            | CHAR(1)            | Not Null             | No   | No   |
| change_current_ind             | Flag indicating whether or not this is an active record.                                                            | CHAR(1)            | Not Null             | No   | No   |
| match_code_addr_lines          | Match code constructed from street address. The match code represents address lines 1 and 2.                        | VARCHAR2(80)       | Null                 | No   | No   |
| match_code_addr_lines          | Match code constructed from street address. The match code represents address lines 1 and 2.                        | VARCHAR2(80)       | Null                 | No   | No   |
| match_code_city                | Match code constructed from street address city name.                                                               | VARCHAR2(30)       | Null                 | No   | No   |
| match_code_city                | Match code constructed from street address city name.                                                               | VARCHAR2(30)       | Null                 | No   | No   |
| match_code_state               | Match code constructed from street address state or province name.                                                  | VARCHAR2(15)       | Null                 | No   | No   |
| match_code_state               | Match code constructed from street address state or province name.                                                  | VARCHAR2(15)       | Null                 | No   | No   |

[Back to index](./index.md)