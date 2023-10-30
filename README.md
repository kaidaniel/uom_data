![schema](schema.dot.png)

# PRODUCT
Example:

|product-id|name|category|start-offer|end-offer|
|----------|----|--------|-----------|---------|
|3|"Club Lloyds"|"SAVINGS-ACCOUNT"|2012-06-01|2013-12-31|
|4|"Club Lloyds"|"SAVINGS-ACCOUNT"|2014-01-01|2014-06-01|
|...|...|...|...|

- **product-id**: A number unique for each row.
- **name**: The name of the product.
- **category**: CURRENT-ACCOUNT or SAVINGS-ACCOUNT or CREDIT-CARD or OVERDRAFT.
- **start-offer**: When the product started being offered in yyyy-mm-dd format.
- **end-offer**: Null or when the product stopped being offered in yyyy-mm-dd format.

# CURRENT-ACCOUNT
Example:

|product-id|interest|monthly-fee|min-deposit|
|----------|--------|-----------|-----------|
|2|0.02|1|100|
|...|...|...|...|

- **product-id**: From PRODUCT. Unique for each row.
- **interest**: Fraction of balance accumulating per year.
- **monthly-fee**: Amount deducted from the account automatically each month.
- **min-deposit**: Smallest amount that can be deposited in a single transaction.

# SAVINGS-ACCOUNT
Example:

|product-id|interest|min-monthly-deposit|max-monthly-deposit|max-withdrawal|
|----------|--------|-------------------|-------------------|--------------|
|1|0.03|1000|100000|30000|
|...|...|...|...|...|

- **product-id**: From PRODUCT. Unique for each row.
- **interest**: Fraction of balance accumulating per year.
- **min-monthly-deposit**: Smallest sum of amounts that need to be deposited per month.
- **max-monthly-deposit**: Largest sum of amounts that can be deposited per month.
- **max-withdrawal**: Largest amount that can be withdrawn in a single transaction.

# CREDIT-CARD

# OVERDRAFT

# CUSTOMER

# ACCOUNT

# MERCHANT

# EVENT

# TRANSACTION