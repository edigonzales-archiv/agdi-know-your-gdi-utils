# agdi-know-your-gdi-utils

```
psql -d postgres -c 'ALTER USER ddluser WITH SUPERUSER;'
```

Erstellt die Datenbank, braucht aber ein `-d`, um sich überhaupt in den Cluster einloggen zu können.
```
pg_restore --no-owner --no-privileges --role=ddluser --exit-on-error -C -d postgres soconfig.dmp
```