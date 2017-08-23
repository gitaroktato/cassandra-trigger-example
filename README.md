# Cassandra trigger example
Table definition is the following
```
CREATE TABLE user_logins (
    user_id bigint,
    login_time timestamp,
    PRIMARY KEY((user_id), login_time)
) WITH CLUSTERING ORDER BY (login_time DESC);
```