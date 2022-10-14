The current accounting setup is the plain text accounting system called beancount. It uses positive numbers for what the business has access to, and negative numbers for what it owes, such as bank debts and our investments.

The five main accounts are:
- Assets (+)
- Liabilities (-)
- Equity (-)
- Income (-)
- Expenses (+)

Accounts are nested in a hierarchy and separated by colons. The names can be arbitrary, but must start with a capital letter.

Examples:

Assets:Bank:Checking
Equity:WillyW

Beancount uses the double entry counting method. Every transaction affects at least two accounts, and they must add to zero. This helps us keep track of what kinds of income and expenses affect the balance and profit, as well as catching simple input errors.
Every transaction is also associated with a date, and has an option for notes. Currency type is arbitrary and required. Commas and currency signs are not supported.

Examples:

2020-1-31 * "Went to Jupiter"
    Assets:Bank:Checking     -400000 USD
    Equity:WillyW                      400000 USD

2020-12-1 * "received nasa's payment for soup"
    Assets:Receivable:NASA   -20000000 USD
    Assets:Bank:Checking         20000000 USD


There are four main financial statements. They are:
- Income statement
- Owners Equity
- Balance sheet
- Cash flow

