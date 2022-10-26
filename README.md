# SQLite3

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
