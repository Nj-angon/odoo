# odoo
1. first copy the .sql file inside postgre bin file
2. go to command prompt and route postgre bin file 
psql -U postgres
CREATE DATABASE mydatabase;
\q
3. createdb -U postgres(owner_name) -O owner_name database_name;
4. psql -U postgres(owner_name) -d mydatabase -f backup_file_name.sql
locate the filestore

#pg_dump -h localhost -U odoo -d Olila_prod -Fc -f /odoo/Olila_prod.sql
#pg_restore -U enterprise -d Olila_prod -Fc -c -v -h localhost -W -p 5432 Olila_prod.sql



