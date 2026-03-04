# Babys First PostgREST Server

# Tutorial
https://docs.postgrest.org/en/v14/tutorials/tut0.html

## Getting Running


### Get datebase running
- Launch Docker Desktop
- `docker run --name tutorial -p 5432:5432  -e POSTGRES_PASSWORD=notused -d postgres:12-bullseye`

### Init database
- `docker exec -it tutorial psql -U postgres`
- Paste contents of `init.sql` file 

## Run PostgREST
`.\postgrest.exe .\tutorial.conf`


## Notes

Couldn't get PostgREST to go into windows path. So just going to keep executable in the repo. to use the PostgREST executable, postgres drivers need to be installed. [https://www.enterprisedb.com/downloads/postgres-postgresql-downloads](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads) 

Use `postgres:12-bullseye` instead of `postgres`. as per [https://stackoverflow.com/questions/76555305/postgres-container-failed-to-start-with-initdb-error-popen-failure-cannot-allo](https://stackoverflow.com/questions/76555305/postgres-container-failed-to-start-with-initdb-error-popen-failure-cannot-allo)





