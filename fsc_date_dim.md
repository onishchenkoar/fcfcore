# FSC_DATE_DIM

---

Calendar date table.

| Column Name           | Column Definition                                                                                                                      | Column Data Type   | Column Null Option   | PK   | FK   |
|:----------------------|:---------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| date_key              | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd | NUMBER(8,0)        | Not Null             | Yes  | No   |
| calendar_date         | The calendar date e.g. 3/18/2003.                                                                                                      | DATE               | Null                 | No   | No   |
| calendar_date_sas     | SAS formatted date.                                                                                                                    | NUMBER(8,0)        | Null                 | No   | No   |
| calendar_date_dmy     | Calendar date in DD/MM/YYYY format                                                                                                     | CHAR(9)            | Null                 | No   | No   |
| day_name              | Which day of the week is it?  e.g. Monday                                                                                              | VARCHAR2(9)        | Null                 | No   | No   |
| day_name_short        | Abbreviated day of week name e.g. Mon                                                                                                  | CHAR(3)            | Null                 | No   | No   |
| day_number_in_month   | Which day of the month it is e.g. 23(rd)                                                                                               | NUMBER(2,0)        | Null                 | No   | No   |
| day_number_in_year    | Which (Julian) day of the year it is e.g. 234                                                                                          | NUMBER(3,0)        | Null                 | No   | No   |
| week_number_in_month  | Which week of the month it is e.g. 3(rd week)                                                                                          | NUMBER(1,0)        | Null                 | No   | No   |
| week_number_in_year   | Which week of the year it is e.g. 52(nd)                                                                                               | NUMBER(2,0)        | Null                 | No   | No   |
| month_number_in_year  | Number of the month e.g. 3(March)                                                                                                      | NUMBER(2,0)        | Null                 | No   | No   |
| month_key             | Foreign Key to the MONTH_DIM table                                                                                                     | NUMBER(6,0)        | Null                 | No   | No   |
| month_and_year        | Month and Year combined e.g. 032003 (March 2003)                                                                                       | CHAR(6)            | Null                 | No   | No   |
| month_name            | Name of Month e.g. March                                                                                                               | VARCHAR2(9)        | Null                 | No   | No   |
| month_name_short      | Abbreviated month name e.g. MAR                                                                                                        | CHAR(3)            | Null                 | No   | No   |
| quarter_name          | Which quarter this date falls in e.g. Q1                                                                                               | CHAR(4)            | Null                 | No   | No   |
| quarter_and_year      | Quarter and Year combined e.g. Q22003                                                                                                  | CHAR(6)            | Null                 | No   | No   |
| month_name_3c         | 3 Char month name e.g. MAR                                                                                                             | CHAR(3)            | Null                 | No   | No   |
| quarter_name_2c       | 2 Character quarter name e.g. Q2                                                                                                       | CHAR(2)            | Null                 | No   | No   |
| quarter_name_4c       | 4 Char quarter name e.g. QTR4                                                                                                          | CHAR(4)            | Null                 | No   | No   |
| year_2c               | Two character year e.g. 03                                                                                                             | CHAR(2)            | Null                 | No   | No   |
| year_4c               | 4 char year e.g. 2003                                                                                                                  | CHAR(4)            | Null                 | No   | No   |
| holiday_ind           | Is this day a holiday for the bank? Y/N                                                                                                | CHAR(1)            | Null                 | No   | No   |
| holiday_name          | If a holiday which holiday is it?  e.g. Independence Day                                                                               | CHAR(9)            | Null                 | No   | No   |
| week_day_ind          | Is this day a weekday? Y/N                                                                                                             | CHAR(1)            | Null                 | No   | No   |
| end_of_month_ind      | Is this day the last day of the month Y/N                                                                                              | CHAR(1)            | Null                 | No   | No   |
| economic_release_desc | release is a economic release by the government. ie. gdp, michigan sentiment, housing starts fed omc etc.                              | VARCHAR2(20)       | Null                 | No   | No   |
| economic_event_desc   | events, are non planned ie. rate changes, etc.                                                                                         | VARCHAR2(20)       | Null                 | No   | No   |

[Back to index](./index.md)