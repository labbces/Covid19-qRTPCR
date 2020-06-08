# Covid19-qRTPCR

This is a simple computational logic infraestructure to read result files produced by a "QuantStudio 12K Flex" RT-qPCR equipment to generate COVID19 diagnostics using 3 target genes and controls.

## Installation

1. Install MySQL, developement used MySQL 8.0.19
2. Create the new database COVID19qRTPCR:

`create database COVID19qRTPCR;`

3. Create a new user ownner of the new database and set a password for them:

`CREATE USER IF NOT EXISTS COVID19qRTPCR@'localhost' IDENTIFIED BY 'password';`

`GRANT ALL PRIVILEGES ON COVID19qRTPCR.* TO 'COVID19qRTPCR'@'localhost';`

4. Create the Schema in your new database

`gunzip -c COVID19qRTPCR.schema-2020-06-08.10\:32.sql.gz |mysql -p -uCOVID19qRTPCR COVID19qRTPCR`

Analysis of qRT-PCR for tests of COVID-19
