# Start psql as postgres user.

```sh
sudo -u postgres psql postgres
```

# Setup a new database (DEVELOPMENT)

Don't grant all privileges in production, of course.

```
postgres=# CREATE USER username WITH PASSWORD 'password';
postgres=# CREATE DATABASE database WITH OWNER username;
postgres=# GRANT ALL PRIVILEGES ON DATABASE database TO username;
```

# Connect to a database

```
\connect database;
```

# List databases

```
\l
```

# List tables

```
\dt
```
