# emergo
Boilerplate for REST API project in SB

```bash
# pull postgres image and run the container
docker run -d --name emergo_postgres -e POSTGRES_USER=emergo_user -e POSTGRES_PASSWORD=emergo_password -e POSTGRES_DB=emergo_db -p 6432:5432 -v ./data/postgres:/var/lib/postgresql/data postgres:latest

# clean and build Spring Boot app
mvn clean && mvn install

# run Spring boot app
mvn spring-boot:run

```