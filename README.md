# Go Migrate Script
Simple bash script to simplify go migrate command. Sometimes migrate command can be long and especially for learner can be difficult to remember. This script might help you learn migration without having to remember long commands like this.
```
migrate create -seq -ext=.sql -dir=./migrations add_movies_check_constraints
```
## Requirement
[Go migrate CLI](https://github.com/golang-migrate/migrate)

## Usage
To get started just run the script. If you don't provide any argument, it will show you usage and flags documentation.
```
./migrate.sh
```
Usage command use the following format:
```
./migrate.sh [--create name] [--migrate] [--rollback number|all] [--goto number] --db [db_dsn]
```
## Flags
| Name                | Description                                    |
| ------------------- | ---------------------------------------------- |
|--create \[name\]    | Create a migration"                            |
|--migrate            | Run migrations up"                             |
|--rollback \[num\]   | Roll back \[num\] migrations"                  |
|--goto \[num\]       | Goto specified \[num\] version of migrations"  | 
|--rollback all       | Roll back all migrations"                      |
|--db \[db_dsn\]      | Specify the database DSN"                      |
