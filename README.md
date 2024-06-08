# odoo
1. first copy the .sql file inside postgre bin file
2. go to command prompt and route postgre bin file 
psql -U postgres
CREATE DATABASE mydatabase;
\q
3. createdb -U postgres(owner_name) -O owner_name database_name;
or
  *createdb -U odoosaas -h 203.190.9.116 -p 6080 dicp.df.daffodil.family
    
6. psql -U postgres(owner_name) -d mydatabase -f backup_file_name.sql
locate the filestore

---- Live Server ------

#sudo -u postgres createdb -O odoo Olila

#pg_dump -h localhost -U odoo -d Olila_prod -Fc -f /odoo/Olila_prod.sql

#pg_restore -U enterprise -d Olila_prod -Fc -c -v -h localhost -W -p 5432 Olila_prod.sql

#pg_restore -U odoo -d Olila_prod -h localhost -p 5432 -W -v /opt/Olila_prod.sql
or
* pg_restore -U odoosaas -d dti.df.daffodil.family -h 203.190.9.116 -p 6080 -W -j 4 -v dti.sql

@Set database user password

#sudo -u postgres psql

#ALTER USER your_username WITH PASSWORD 'your_new_password';

#sudo tail -f /var/log/odoo/odoo-server.log


