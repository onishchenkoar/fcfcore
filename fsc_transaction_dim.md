# FSC_TRANSACTION_DIM

[Back to index](./index.md)

---

A supplementary table to the transaction facts used to capture additional, typically verbose, data that about a transaction.  Storing this data here helps keep the fact table "skinny" and therefore smaller than they would otherwise be.

| Column Name                  | Column Definition                                                                                                                                                                                                              | Column Data Type   | Column Null Option   | PK   | FK   |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|:---------------------|:-----|:-----|
| transaction_key              | Surrogate key..                                                                                                                                                                                                                | NUMBER(12)         | Not Null             | Yes  | No   |
| segment_id                   | Multibank configurations use this column to indicate which bank the record belongs to.                                                                                                                                         | VARCHAR2(128)      | Not Null             | Yes  | No   |
| date_key                     | Note: this is normally a system-generated surrogate key, but for performance reasons we are using a numeric form of the date: yyyymmdd This column has been added to this table to enable table partitioning.                  | NUMBER(8,0)        | Not Null             | No   | No   |
| transaction_reference_number | Source system's transaction identifier e.g. deposit number                                                                                                                                                                     | VARCHAR2(50)       | Not Null             | No   | No   |
| transaction_description      | Free form text description of trade.                                                                                                                                                                                           | VARCHAR2(255)      | Null                 | No   | No   |
| security_name                | Name of the equity, bond, currency etc bought or sold.  Could use ticker if preferred.                                                                                                                                         | VARCHAR2(35)       | Null                 | No   | No   |
| deal_number                  | Number identifying a trade plus associated settlements.  e.g. Trade is to buy 1mm Euros; settled with two wires each of $500K.  All three transactions are part of the same deal and therefore will have the same deal number. | VARCHAR2(35)       | Null                 | No   | No   |
| check_number                 | The check number of the transaction.                                                                                                                                                                                           | VARCHAR2(10)       | Null                 | No   | No   |
| mechanism_id                 | Contains the identifier corresponding to the mechanism description in the FSC_TRANSACTION_TYPE_DIM table. For example if the transaction is remote deposit, the mechanism id will contain the terminal number.                 | VARCHAR2(40)       | Null                 | No   | No   |

[Back to index](./index.md)