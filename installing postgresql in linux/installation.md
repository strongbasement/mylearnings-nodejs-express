### step 1:
```
sudo apt-get update
```
### step 2:

```
sudo apt install postgresql postgresql-contrib 
```

### step 3 :check

```
sudo systemctl status postgresql

```
### step 4:

```
sudo su - postgres
```

### step 5: selecting version

```

select version();
```
### step 6
```
alter user postgres with password 'anypassword';
```

### step 7: create databases
```
create database dbname;
```

### step 8: list databases
```
\l
```
### step 9: connect to the database
```
\c  dbname;

```
### create a new user

```
create user prabhusample with password 'lion@123';

```
###   check the numbers of users by 

```
\du
```