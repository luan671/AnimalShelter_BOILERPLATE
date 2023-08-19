### The Sevaa Animal Shelter

# Requirements for local setup:
php8
Composer2 (preferred)
ddev

//Env variables should be modified within the .env file in root dir
//All plugins are nested&installed through composer

# Running the site locally:
- Docker needs to be running
- Obtain the .env file and place in root dir, edit as needed
- Run to initialize
```bash
ddev config
```
- Run to start the project
```bash
ddev start
```
- Obtain the custom block plugin from https://github.com/luan671/Custom-Testimonial-Block place into /plugin accordingly
- Decompress the backup database then place into the db contaniner
- Run the .sql against WordPress db (default name 'db'):
```sql
mysql db < ${some_backup}.sql
```
