# backup-psql
Small bash script for backing up postgresql databases.

```
Usage: 
    backup-psql [OPTIONS]

Options:
    --help
    -h=, --host=<ip|domain>     PostgreSQL server host
                                If not specified then localhost will be used.
    -p=, --port=<port>          PostgreSQL server port. 
                                If not specified then standart port 5432 will be used.
    -u=, --user=<DB user>       PostgreSQL server user
    -ps=, --password=<password> PostgreSQL server user password
    -bp=, --backup_path=<path>  Path to backup folder
                                If not specified then current working directory will be used.
    -d=, --db_name=<DB name>    Name of PostgreSQL Data Base. 
                                If not specified then all data bases will be backuped.

Example: 
    backup-psql -h=127.0.0.1 -p=5432 -u=dbuser -ps=1234 -bp=./ -d=mydatabase
    backup-psql -u=dbuser -ps=1234
```
