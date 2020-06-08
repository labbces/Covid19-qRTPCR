# Covid19-qRTPCR

## Installation

1. Install MySQL, developement used MySQL 8.0.19
2. Create the new database COVID19qRTPCR:

`create database COVID19qRTPCR;`

3. Create a new user ownner of the new database and set a password for them:

`CREATE USER IF NOT EXISTS COVID19qRTPCR@'localhost' IDENTIFIED BY 'password';`

`GRANT ALL PRIVILEGES ON COVID19qRTPCR.* TO 'COVID19qRTPCR'@'localhost';`

Analysis of qRT-PCR for tests of COVID-19
