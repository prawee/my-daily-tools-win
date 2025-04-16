# How to install `MariaDB` with scoop

## Searching
```bash
PS C:\> scoop search mariadb
Results from local buckets...

Name    Version Source Binaries
----    ------- ------ --------
mariadb 11.7.2  main


PS C:\>
```

## Install
```bash
PS C:\> scoop install mariadb
Installing 'mariadb' (11.7.2) [64bit] from 'main' bucket
mariadb-11.7.2-winx64.zip (87.9 MB) [====================================>                               ]  23%
```
```bash
Checking hash of mariadb-11.7.2-winx64.zip ... ok.=============================================================================================] 100%
Extracting mariadb-11.7.2-winx64.zip ... done.
Linking ~\scoop\apps\mariadb\current => ~\scoop\apps\mariadb\11.7.2
Creating shim for 'aria_chk'.
Creating shim for 'aria_dump_log'.
Creating shim for 'aria_ftdump'.
Creating shim for 'aria_pack'.
Creating shim for 'aria_read_log'.
Creating shim for 'innochecksum'.
Creating shim for 'myisamchk'.
Creating shim for 'myisamlog'.
Creating shim for 'myisampack'.
Creating shim for 'myisam_ftdump'.
Creating shim for 'mysql'.
Creating shim for 'mysqladmin'.
Creating shim for 'mysqlbinlog'.
Creating shim for 'mysqlcheck'.
Creating shim for 'mysqld'.
Creating shim for 'mysqldump'.
Creating shim for 'mysqlimport'.
Creating shim for 'mysqlshow'.
Creating shim for 'mysqlslap'.
Creating shim for 'mysql_install_db'.
Creating shim for 'mysql_plugin'.
Creating shim for 'mysql_tzinfo_to_sql'.
Creation of the database was successful
WARN  Database has been initialized (username: root, password: <blank>)
done.
'mariadb' (11.7.2) was installed successfully!
Notes
-----
Run 'mysqld --standalone' or 'mysqld --console' to start the Database,
or run following command as administrator to register MariaDB as a service. See: https://mariadb.com/kb/en/library/mysql_install_dbexe/

mysql_install_db --service=MariaDB --password=NewRootPassword

To stop and/or delete the Service run 'sc stop MariaDB' and 'sc delete MariaDB'.
PS C:\>
```

## Try to console
### Start database first
```bash
PS C:\> mysqld --console   
2025-04-14 16:30:18 0 [Note] Starting MariaDB 11.7.2-MariaDB source revision 80067a69feaeb5df30abb1bfaf7d4e713ccbf027 server_uid fHIURoylFP9kr3hyNTbk0ZNMSYE= as process 2988
2025-04-14 16:30:18 0 [Note] InnoDB: Compressed tables use zlib 1.3.1
2025-04-14 16:30:18 0 [Note] InnoDB: Number of transaction pools: 1
2025-04-14 16:30:18 0 [Note] InnoDB: Using crc32 + pclmulqdq instructions
2025-04-14 16:30:18 0 [Note] InnoDB: Initializing buffer pool, total size = 128.000MiB, chunk size = 2.000MiB
2025-04-14 16:30:18 0 [Note] InnoDB: Completed initialization of buffer pool
2025-04-14 16:30:18 0 [Note] InnoDB: File system buffers for log disabled (block size=4096 bytes)
2025-04-14 16:30:18 0 [Note] InnoDB: End of log at LSN=47875
2025-04-14 16:30:18 0 [Note] InnoDB: Opened 3 undo tablespaces
2025-04-14 16:30:18 0 [Note] InnoDB: 128 rollback segments in 3 undo tablespaces are active.
2025-04-14 16:30:18 0 [Note] InnoDB: Setting file './ibtmp1' size to 12.000MiB. Physically writing the file full; Please wait ...
2025-04-14 16:30:18 0 [Note] InnoDB: File './ibtmp1' size is now 12.000MiB.
2025-04-14 16:30:18 0 [Note] InnoDB: log sequence number 47875; transaction id 15
2025-04-14 16:30:18 0 [Note] Plugin 'FEEDBACK' is disabled.
2025-04-14 16:30:18 0 [Note] InnoDB: Loading buffer pool(s) from C:\Users\Admin\scoop\apps\mariadb\current\data\ib_buffer_pool
2025-04-14 16:30:18 0 [Note] mysqld.exe: SSPI: using principal name 'localhost', mech 'Negotiate'
2025-04-14 16:30:18 0 [Note] InnoDB: Buffer pool(s) load completed at 250414 16:30:18
2025-04-14 16:30:20 0 [Note] Server socket created on IP: '::'.
2025-04-14 16:30:20 0 [Note] Server socket created on IP: '0.0.0.0'.
2025-04-14 16:30:20 0 [Note] mysqld.exe: Event Scheduler: Loaded 0 events
2025-04-14 16:30:20 0 [Note] C:\Users\Admin\scoop\apps\mariadb\current\bin\mysqld.exe: ready for connections.
Version: '11.7.2-MariaDB'  socket: ''  port: 3306  mariadb.org binary distribution
```

### Connect
```bash
PS C:\> mysql -u root -p
Enter password: <blank>
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 5
Server version: 11.7.2-MariaDB mariadb.org binary distribution

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]>
```

## Uninstall
```bash
PS C:\> scoop uninstall mariadb
Uninstalling 'mariadb' (11.7.2).
Removing shim 'aria_chk.shim'.
Removing shim 'aria_chk.exe'.
Removing shim 'aria_dump_log.shim'.
Removing shim 'aria_dump_log.exe'.
Removing shim 'aria_ftdump.shim'.
Removing shim 'aria_ftdump.exe'.
Removing shim 'aria_pack.shim'.
Removing shim 'aria_pack.exe'.
Removing shim 'aria_read_log.shim'.
Removing shim 'aria_read_log.exe'.
Removing shim 'innochecksum.shim'.
Removing shim 'innochecksum.exe'.
Removing shim 'myisamchk.shim'.
Removing shim 'myisamchk.exe'.
Removing shim 'myisamlog.shim'.
Removing shim 'myisamlog.exe'.
Removing shim 'myisampack.shim'.
Removing shim 'myisampack.exe'.
Removing shim 'myisam_ftdump.shim'.
Removing shim 'myisam_ftdump.exe'.
Removing shim 'mysql.shim'.
Removing shim 'mysql.exe'.
Removing shim 'mysqladmin.shim'.
Removing shim 'mysqladmin.exe'.
Removing shim 'mysqlbinlog.shim'.
Removing shim 'mysqlbinlog.exe'.
Removing shim 'mysqlcheck.shim'.
Removing shim 'mysqlcheck.exe'.
Removing shim 'mysqld.shim'.
Removing shim 'mysqld.exe'.
Removing shim 'mysqldump.shim'.
Removing shim 'mysqldump.exe'.
Removing shim 'mysqlimport.shim'.
Removing shim 'mysqlimport.exe'.
Removing shim 'mysqlshow.shim'.
Removing shim 'mysqlshow.exe'.
Removing shim 'mysqlslap.shim'.
Removing shim 'mysqlslap.exe'.
Removing shim 'mysql_install_db.shim'.
Removing shim 'mysql_install_db.exe'.
Removing shim 'mysql_plugin.shim'.
Removing shim 'mysql_plugin.exe'.
Removing shim 'mysql_tzinfo_to_sql.shim'.
Removing shim 'mysql_tzinfo_to_sql.exe'.
Removing shim 'mysql_upgrade.shim'.
Removing shim 'mysql_upgrade.exe'.
Removing shim 'mysql_upgrade_service.shim'.
Removing shim 'mysql_upgrade_service.exe'.
Removing shim 'my_print_defaults.shim'.
Removing shim 'my_print_defaults.exe'.
Unlinking ~\scoop\apps\mariadb\current
'mariadb' was uninstalled.
PS C:\>
```
