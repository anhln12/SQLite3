# SQLite3

# refe https://www.sqlitetutorial.net/

# Install

1. Download the Source Code

Create a new directory for SQLite3
```
# mkdir sqlite3 && cd sqlite3
```

Navigate to https://www.sqlite.org/download.html and copy the link to the latest code, which will be named:
```
# sqlite-autoconf-<version>.tar.gz
```

Download it using wget command and extract is using tar
```
# wget [link to sqlite-autoconf-<version>.tar.gz]
# tar xvfz sqlite-autoconf-<version>.tar.gz
```

Build & Install SQLite3
```
# cd sqlite-autoconf-<version>
# ./configure
# make
# make install
```
Verify the Installation
```
# sqlite3 --version
```

# Connect SQLite3
https://sqlitestudio.pl/


# Export SQLite Database to a CSV file using sqlite 3 tool
SQLite project provides you with command-line program called sqlite3. By using the sqlite3 tool, you can use the SQL statements.

To export data from the SQLite database to a CSV file, you use these steps:
1. Turn on/off the header of the result set using the .header on command.
2. Set the output mode to CSV to intruct the sqlite3 tool to issue the result in the CSV mode.
3. Send to output to a CSV file
4. Issue the query to select data from the customers table and export it to the data.csv file

```
[root@xyz]# sqlite3 /home/ht_anhln/database.db 
SQLite version 3.7.17 2013-05-20 00:56:22
Enter ".help" for instructions
Enter SQL statements terminated with a ";"
sqlite> .header off
sqlite> .mode csv
sqlite> .output data.csv
sqlite> select email from users where email like '%@%';
sqlite> .quit
```
