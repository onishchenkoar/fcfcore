# FSC_TIME_DIM

---

The seconds in a day.

[Back to index](./index.md)

| Column Name     | Column Definition                                                                                                    | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------|:---------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **TIME_KEY**    | System generated surrogate key.  Is NOT of form hhmmss in tables though it does come in that way in the stage files. | NUMBER(6)          | Not Null             | Yes  | No   |
| **TIME_HHMMSS** | hour,min,sec                                                                                                         | CHAR(6)            | Null                 | No   | No   |
| **TIME_HH**     | hour                                                                                                                 | CHAR(2)            | Null                 | No   | No   |
| **TIME_MM**     | minutes                                                                                                              | CHAR(2)            | Null                 | No   | No   |
| **TIME_SS**     | seconds                                                                                                              | CHAR(2)            | Null                 | No   | No   |
| **TIME_AM_PM**  | am or pm                                                                                                             | CHAR(2)            | Null                 | No   | No   |

[Back to index](./index.md)