FROM postgres:10.3
# creates /docker-entrypoint-initdb.d/tables folder in container
ADD /tables/ /docker-entrypoint-initdb.d/tables/
ADD deploy_schemas.sql /docker-entrypoint-initdb.d/