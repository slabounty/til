# Restart Database on Mac

Sometimes when a mac restarts, it does not restart the database
properly. It will look like it's running, but nothing will be able to
connect.

```
rm /usr/local/var/postgres/postmaster.pid
brew services restart postgresql
```
