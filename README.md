# snl-data-diff
Ship N Learn Data Diff


### What is data diff?
- Its a [python library](https://github.com/datafold/data-diff) to be able to perform [data reconciliation](https://www.guru99.com/what-is-data-reconciliation.html)
- Uses MD5 Hashing to compare data in two different sources, and since we are only pulling primary key and also the `updated_at` column, the data scan is very minimal.

### When to use data diff?
- When you suspect theres only a small difference in data between source and destination, else it is going to have to scan through each block of data, and it will still be relatively slow

- On how to improve performance, please refer to the [source library](https://github.com/datafold/data-diff#performance-considerations)
