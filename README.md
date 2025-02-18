## Add local cliente postgresql for dbeaver
1. ```sudo apt install postgresql-client```

Note: Then in DBeaver, go to Database->Driver Manager, choose "PostgreSQL" then "Edit" then navigate to the "Native Client" tab, then "Add Home" and choose /usr/bin as the location, since it's where pg_dump and pg_restore are installed. Alternatively, you may choose /usr/lib/postgresql/<version>/bin where <version> is your PostgreSQL version, if you have several versions installed and the automatic selection by /usr/bin/pg_dump doesn't work for you. https://serverfault.com/questions/1101295/not-able-to-backup-of-postgres-db-from-dbeaver
