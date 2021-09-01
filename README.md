# apache-guacamole-docker-compose
Apache Guacamole in Docker Compose

## Sources
- Guacamole: https://guacamole.apache.org/ 
- Inspiration by: https://github.com/reisbel/guacamole-docker-compose
- Documentation: https://guacamole.apache.org/doc/gug/ 

## Running the docker-compose
- Clone the repo
- Go to `apache-guacamole-docker-compose/docker` folder
- Change the username and password for Postgres DB that are stored inside environment file (`.env`)
- Initialize the Database by running this command:
```
docker-compose up init-guacamole-db
```
- Start guacamole: 
```
docker-compose up -d
```

Guacamole will run on port 8090.


## Post-installation
- change the default password and username
-- default username: `guacadmin`
-- default password: `guacadmin`
- use a reverse-proxy to point to the guacamole app
- Consult the documentation for further details: https://guacamole.apache.org/doc/gug/ 
