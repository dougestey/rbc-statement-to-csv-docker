# RBC Statement To CSV

This program will read transaction data out of RBC credit card statements and put them in a .csv file with the following columns:

- Transaction Date
- Posting Date
- Description
- Amount
- Amount In Foreign Currency
- Foreign Currency
- Exchange Rate

## Requirements

- Docker version 23.0.3, build 3e7cbfd
- docker-compose version 1.27.4, build 40524192 

## Use

- Drop all PDF statements into the `/app` directory. The program will read all transactions, sort them, and consolidate them into a single .csv file called transactions.csv.
- `docker-compose up`
- You'll see the CSV appear in `/app`.
