Log in with default user

    sudo -u postgres psql siri
	 
	 
Add user:

	create role obus with login password 'obus';
	
Grant permissions:
	 GRANT ALL PRIVILEGES ON ALL TABLES IN SCHEMA public TO obus;
	GRANT USAGE, SELECT ON ALL SEQUENCES IN SCHEMA public to obus;
	
Change password:

     ALTER USER "user_name" WITH PASSWORD 'new_password';

List users:

    \du
	  

List tables:

	\dt
	  
create database:

	create database siri;

import schema:

	sudo -u postgres psql siri postgres < schema.sql

