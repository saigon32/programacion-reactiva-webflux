# programacion-reactiva-webflux
programacion-reactiva-webflux excelente explicacion de crud reactivo con mono y flux usando postgres


manual de referencia:
https://www.cleveritgroup.com/blog/programacion-reactiva-con-spring-webflux-parte-2

crear contenedor de postgres en docker:
docker run --name basic-postgres --rm -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=4y7sV96vA9wv46VR -e PGDATA=/var/lib/postgresql/data/pgdata -v /tmp:/var/lib/postgresql/data -p 5432:5432 -it postgres:14.1-alpine

creacion de la tabla:
CREATE TABLE public.book
( 
	id integer  NOT NULL,
	title text  NOT NULL,
	author text NOT NULL
)
acceder al microservicio:
http://localhost:8081/api/func/books/11
