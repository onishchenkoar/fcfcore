# FSC_DATE_DIM

---

Calendar date table.

[Back to index](./index.md)

| Column Name               | Column Definition                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:--------------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| **DATE_KEY**              | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | NUMBER(8,0)        | Not Null             | Yes  | No   |
| **CALENDAR_DATE**         | The calendar date e.g. 3/18/2003.                                                                                                      | DATE               | Null                 | No   | No   |
| **CALENDAR_DATE_SAS**     | SAS formatted date.                                                                                                                    | NUMBER(8,0)        | Null                 | No   | No   |
| **CALENDAR_DATE_DMY**     | Calendar date in DD/MM/YYYY format                                                                                                     | CHAR(9)            | Null                 | No   | No   |
| **DAY_NAME**              | Which day of the week is it?  e.g. Monday                                                                                              | VARCHAR2(9)        | Null                 | No   | No   |
| **DAY_NAME_SHORT**        | Abbreviated day of week name e.g. Mon                                                                                                  | CHAR(3)            | Null                 | No   | No   |
| **DAY_NUMBER_IN_MONTH**   | Which day of the month it is e.g. 23(rd)                                                                                               | NUMBER(2,0)        | Null                 | No   | No   |
| **DAY_NUMBER_IN_YEAR**    | Which (Julian) day of the year it is e.g. 234                                                                                          | NUMBER(3,0)        | Null                 | No   | No   |
| **WEEK_NUMBER_IN_MONTH**  | Which week of the month it is e.g. 3(rd week)                                                                                          | NUMBER(1,0)        | Null                 | No   | No   |
| **WEEK_NUMBER_IN_YEAR**   | Which week of the year it is e.g. 52(nd)                                                                                               | NUMBER(2,0)        | Null                 | No   | No   |
| **MONTH_NUMBER_IN_YEAR**  | Number of the month e.g. 3(March)                                                                                                      | NUMBER(2,0)        | Null                 | No   | No   |
| **MONTH_KEY**             | Foreign Key to the [FSC_MONTH_DIM](./fsc_month_dim.md) table                                                                                                     | NUMBER(6,0)        | Null                 | No   | No   |
| **MONTH_AND_YEAR**        | Month and Year combined e.g. 032003 (March 2003)                                                                                       | CHAR(6)            | Null                 | No   | No   |
| **MONTH_NAME**            | Name of Month e.g. March                                                                                                               | VARCHAR2(9)        | Null                 | No   | No   |
| **MONTH_NAME_SHORT**      | Abbreviated month name e.g. MAR                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| **QUARTER_NAME**          | Which quarter this date falls in e.g. Q1                                                                                               | CHAR(4)            | Null                 | No   | No   |
| **QUARTER_AND_YEAR**      | Quarter and Year combined e.g. Q22003                                                                                                  | CHAR(6)            | Null                 | No   | No   |
| **MONTH_NAME_3C**         | 3 Char month name e.g. MAR                                                                                                             | CHAR(3)            | Null                 | No   | No   |
| **QUARTER_NAME_2C**       | 2 Character quarter name e.g. Q2                                                                                                       | CHAR(2)            | Null                 | No   | No   |
| **QUARTER_NAME_4C**       | 4 Char quarter name e.g. QTR4                                                                                                          | CHAR(4)            | Null                 | No   | No   |
| **YEAR_2C**               | Two character year e.g. 03                                                                                                             | CHAR(2)            | Null                 | No   | No   |
| **YEAR_4C**               | 4 char year e.g. 2003                                                                                                                  | CHAR(4)            | Null                 | No   | No   |
| **HOLIDAY_IND**           | Is this day a holiday for the bank? Y/N                                                                                                | CHAR(1)            | Null                 | No   | No   |
| **HOLIDAY_NAME**          | If a holiday which holiday is it?  e.g. Independence Day                                                                               | CHAR(9)            | Null                 | No   | No   |
| **WEEK_DAY_IND**          | Is this day a weekday? Y/N                                                                                                             | CHAR(1)            | Null                 | No   | No   |
| **END_OF_MONTH_IND**      | Is this day the last day of the month Y/N                                                                                              | CHAR(1)            | Null                 | No   | No   |
| **ECONOMIC_RELEASE_DESC** | Release is a economic release by the government, i.e. gdp, michigan sentiment, housing starts fed omc etc.                              | VARCHAR2(20)       | Null                 | No   | No   |
| **ECONOMIC_EVENT_DESC**   | Events, are non planned ie. rate changes, etc.                                                                                         | VARCHAR2(20)       | Null                 | No   | No   |

[Back to index](./index.md)
