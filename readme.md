#create postgres container using docker command

docker run -d --name my_postgres -v my_dbdata:/var/lib/postgresql/data -p 54320:5432 postgres:11

#create postgres container using docker-compose

docker-compose up -d

#connect postgres container

docker exec -it my_postgres psql -U postgres
