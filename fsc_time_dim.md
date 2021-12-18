# FSC_TIME_DIM

---

The seconds in a day.

| Attribute Name   | Attribute Definition                                                                                                 | Column Data Type   | Column Null Option   | Column Is PK   | Column Is FK   |
|:-----------------|:---------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:---------------|:---------------|
| time_key         | System generated surrogate key.  Is NOT of form hhmmss in tables though it does come in that way in the stage files. | NUMBER(6)          | Not Null             | Yes            | No             |
| time_hhmmss      | hour,min,sec                                                                                                         | CHAR(6)            | Null                 | No             | No             |
| time_hh          | hour                                                                                                                 | CHAR(2)            | Null                 | No             | No             |
| time_mm          | minutes                                                                                                              | CHAR(2)            | Null                 | No             | No             |
| time_ss          | seconds                                                                                                              | CHAR(2)            | Null                 | No             | No             |
| time_am_pm       | am or pm                                                                                                             | CHAR(2)            | Null                 | No             | No             |

[Back to index](./index.md)