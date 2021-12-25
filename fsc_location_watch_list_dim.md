# FSC_LOCATION_WATCH_LIST_DIM

---

Countries appearing on selected country watch lists (e.g. NCCT list).

[Back to index](./index.md)

| Column Name                    | Column Definition                                                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:-------------------------------|:-------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **LOCATION_WATCH_LIST_KEY**    | Surrogate key.                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| **LOCATION_WATCH_LIST_NUMBER** | Natural key from watch list provider                                     | VARCHAR2(35)       | Not Null             | No   | No   |
| **WATCH_LIST_NAME**            | Name of watch list.                                                      | CHAR(4)            | Not Null             | No   | No   |
| **PROGRAM**                    | Programs associated with this list (e.g. OFAC~ USDOJ~INTERPOL).           | VARCHAR2(20)       | Null                 | No   | No   |
| **COUNTRY_CODE**               | Country code of location.                                                | CHAR(3)            | Null                 | No   | No   |
| **COUNTRY_NAME**               | Country name of location.                                                | VARCHAR2(255)      | Null                 | No   | No   |
| **MATCH_CODE_COUNTRY_NAME**    | Match code generated from country name                                   | VARCHAR2(15)       | Null                 | No   | No   |
| **CREATE_DATE**                | Date record was created                                                  | DATE               | Null                 | No   | No   |
| **UPDATE_DATE**                | Date record was last updated                                             | DATE               | Null                 | No   | No   |
| **EXCLUDE_IND**                | Flag which user can set to exclude this entity from watch list analysis. | CHAR(1)            | Not Null             | No   | No   |
| **CHANGE_BEGIN_DATE**          | First date record is effective.                                          | DATE               | Not Null             | No   | No   |
| **CHANGE_END_DATE**            | Last date record is effective.                                           | DATE               | Not Null             | No   | No   |
| **CHANGE_CURRENT_IND**         | Y or N flag indicating whether or not this is the current record.        | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)
