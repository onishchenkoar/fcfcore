# FSC_LOCATION_WATCH_LIST_DIM

---

Countries appearing on selected country watch lists (e.g. NCCT list).

| Attribute Name             | Attribute Definition                                                     | Column Name                | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:---------------------------|:-------------------------------------------------------------------------|:---------------------------|:-------------------|:---------------------|:---------------|:---------------|
| location_watch_list_key    | Surrogate key.                                                           | location_watch_list_key    | NUMBER(12)         | Not Null             | Yes            | No             |
| location_watch_list_number | Natural key from watch list provider                                     | location_watch_list_number | VARCHAR2(35)       | Not Null             | No             | No             |
| watch_list_name            | Name of watch list.                                                      | watch_list_name            | CHAR(4)            | Not Null             | No             | No             |
| program                    | Programs associated with this list(e.g. OFAC~ USDOJ~INTERPOL).           | program                    | VARCHAR2(20)       | Null                 | No             | No             |
| country_code               | Country code of location.                                                | country_code               | CHAR(3)            | Null                 | No             | No             |
| country_name               | Country name of location.                                                | country_name               | VARCHAR2(255)      | Null                 | No             | No             |
| match_code_country_name    | Match code generated from country name                                   | match_code_country_name    | VARCHAR2(15)       | Null                 | No             | No             |
| create_date                | Date record was created                                                  | create_date                | DATE               | Null                 | No             | No             |
| update_date                | Date record was last updated                                             | update_date                | DATE               | Null                 | No             | No             |
| exclude_ind                | Flag which user can set to exclude this entity from watch list analysis. | exclude_ind                | CHAR(1)            | Not Null             | No             | No             |
| change_begin_date          | First date record is effective.                                          | change_begin_date          | DATE               | Not Null             | No             | No             |
| change_end_date            | Last date record is effective.                                           | change_end_date            | DATE               | Not Null             | No             | No             |
| change_current_ind         | Y or N flag indicating whether or not this is the current record.        | change_current_ind         | CHAR(1)            | Not Null             | No             | No             |

[Back to index](./README.md)