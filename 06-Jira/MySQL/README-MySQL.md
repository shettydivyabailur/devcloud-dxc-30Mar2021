```
# Note: Please append the following lines in mysqld section for JIRA Configuration.
# DB Create Step you will find in assocate history.
# Plase make sure your DB Bind Address for extrnal communication. 
```

# DB Creation:
```
mysql -u root -p 
CREATE USER 'jira'@'%' IDENTIFIED BY 'redhat';
CREATE DATABASE jira CHARACTER SET utf8mb4 COLLATE utf8mb4_bin;
GRANT ALL PRIVILEGES ON jira.* TO 'jira'@'%';
quit;
```

# Sample MySQL DB File
```
[mysqld]
default-storage-engine=INNODB
innodb_default_row_format=DYNAMIC
character_set_server=utf8mb4
innodb_large_prefix=ON
innodb_file_format=Barracuda
innodb_log_file_size=2G
collation-server=utf8mb4_bin
max_allowed_packet=256M
transaction-isolation=READ-COMMITTED
binlog_format=row
```
