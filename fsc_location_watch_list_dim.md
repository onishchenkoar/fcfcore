# **FSC_LOCATION_WATCH_LIST_DIM**

---

Countries appearing on selected country watch lists (e.g. NCCT list).

[Back to index](./index.md)

| Column Name                | Column Definition                                                        | Column Data Type   | Column Null Option   | PK   | FK   |
|:---------------------------|:-------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| location_watch_list_key    | Surrogate key.                                                           | NUMBER(12)         | Not Null             | Yes  | No   |
| location_watch_list_number | Natural key from watch list provider                                     | VARCHAR2(35)       | Not Null             | No   | No   |
| watch_list_name            | Name of watch list.                                                      | CHAR(4)            | Not Null             | No   | No   |
| program                    | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).           | VARCHAR2(20)       | Null                 | No   | No   |
| country_code               | Country code of location.                                                | CHAR(3)            | Null                 | No   | No   |
| country_name               | Country name of location.                                                | VARCHAR2(255)      | Null                 | No   | No   |
| match_code_country_name    | Match code generated from country name                                   | VARCHAR2(15)       | Null                 | No   | No   |
| create_date                | Date record was created                                                  | DATE               | Null                 | No   | No   |
| update_date                | Date record was last updated                                             | DATE               | Null                 | No   | No   |
| exclude_ind                | Flag which user can set to exclude this entity from watch list analysis. | CHAR(1)            | Not Null             | No   | No   |
| change_begin_date          | First date record is effective.                                          | DATE               | Not Null             | No   | No   |
| change_end_date            | Last date record is effective.                                           | DATE               | Not Null             | No   | No   |
| change_current_ind         | Y or N flag indicating whether or not this is the current record.        | CHAR(1)            | Not Null             | No   | No   |

[Back to index](./index.md)