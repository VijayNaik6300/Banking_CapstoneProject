# Banking Application - Fixed Version

Fixed issues include:
- Customer number generation and persistence.
- Date of birth persistence and PATCH support.
- Account update no longer changes balance.
- Account numbers no longer depend on row count.
- Pessimistic locking for financial operations and consistent lock order for transfers.
- Optimistic locking on accounts using @Version.
- Opening balances are recorded as deposit transactions.
- Inactive customers/accounts cannot perform financial operations.
- Validation for positive monetary values and max two decimal places.
- Corrected misplaced AccountResponse and TransactionRepository classes.
- Demo data includes valid customer numbers and DOBs.
- POST create endpoints return HTTP 201.
- Old H2 runtime database removed so a fresh schema is created.
