# Project: Build a Data Mart in SQL

This setup manual is designed for Linux, specifically tested on *Ubuntu 24.04 LTS* and *mysql Ver 8.0.42-0ubuntu0.24.04.2 for Linux on x86_64 ((Ubuntu))*. Follow the installation steps carefully. 
## 1. Prerequisit installation

### First open the terminal (Ctrl + Alt + t) and check if MySQL is already installed and which vesion it has:

``` 
sudo mysql --version
```
### If MySQL is not installed yet:

```
sudo apt install -y mysql-server 
```
MySQL secure installation (optional):

```
sudo mysql_secure_installation
```

### MySQL secure setup
| configuration| option |
| ------ | ----------- |
| VALIDATE PASSWORD COMPONENT| `no` (if testing in a sandbox environment)|
| Remove anonymous users? | `yes` |
| Disallow root login remotely?| `yes`|
| Remove test database and access to it? | `yes` |
| Reload privilege tables now? | `yes`|

## 2. SQL file execution

### Navigate into the project folder where the .sql file is located:

``` 
cd 03-Finalisation/
```

### Login into MySQL Server:

``` 
sudo mysql
```
### In the MySQL terminal:

``` 
source Fauser-Juri_32207633_DLBDSPBDM01_P2_S_Code.sql;
```
