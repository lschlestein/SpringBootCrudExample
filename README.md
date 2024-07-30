#Spring Boot CRUD
Esse repositório implementa um exemplo simples de uma aplicação MVC com um CRUD.
Para rodar esse projeto é necessário configurar uma database de nome CRUD, no Postgres. Verificar usuário e senha (user: postgres, senha:1234)
Também é possível remover a dependência do Postgres do arquivo Pom.xml, e adicionar o H2, que implementa uma DB em memória.

application.properties
```
spring.application.name=CRUD
#Update the database schema based on the entities create-drop / update
spring.jpa.hibernate.ddl-auto= update
#create database if not exists mysql true spring boot
#spring.datasource.url=jdbc:mysql://localhost:3306/CRUD?createDatabaseIfNotExist=true
spring.datasource.url=jdbc:postgresql://localhost:5432/CRUD
#DB User
spring.datasource.username=postgres
#DB password
spring.datasource.password=1234
```
