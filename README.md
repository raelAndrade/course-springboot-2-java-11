# Workshop criação de WebServices com Spring Boot e JPA/Hibernate

#### Nesse workshop foram aplicados as seguintes funcionalidades:

* Métodos HTTP - GET/POST/PUT/DELETE
* Criação de Manipulador de Exception personalizadas

#### Tecnologias utilizadas:

* Spring Boot
* Spring Data JPA
* Banco de dados relacional - Postgres e H2

#### Ferramentas para teste da API e Banco de dados:

* Insomnia
* DBeaver
* PGAdmin 4

#### Ferramentas de desenvolvimento:

* Intellij

#### Conceitos aplicados nas fase de desenvolvimento:

* Implementação de modelo de domínio
* Instância de Domínio
* Estrutura de camadas lógicas: Resource, Service e Repository
* CRUD - Criar, Recuperar, Atualizar e Deletar
* Tratamento de Exceções
* Dev profile

#### Deploy da API no Heroku

* Criação de app no dashboard da heroku
* Configuração de variáveis de ambiente
* Criação da base de dados Postgres
* Implantação da API REST

#### Users - Endpoints

```js
@GET todos

curl -X GET \
  https://api-rest-product-order.herokuapp.com/users \
  -H 'cache-control: no-cache' \
```

```js
@GET por id

curl -X GET \
  https://api-rest-product-order.herokuapp.com/users/1 \
  -H 'cache-control: no-cache' \
```

```js
@POST

curl -X POST \
  https://api-rest-product-order.herokuapp.com/users \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -d '{
	"name": "Maria Brown",
	"email": "maria@gmail.com",
	"phone": "977557799",
	"password": "123456"
  }'
```

```js
@PUT

curl -X PUT \
  https://api-rest-product-order.herokuapp.com/users/1 \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -d '{
        "name": "Maria José",
	      "email": "maria.jose@gmail.com",
	      "phone": "999990000",
	      "password": "123456"
  }'
```

```js
@DELETE

curl -X DELETE \
  https://api-rest-product-order.herokuapp.com/users/1 \
  -H 'cache-control: no-cache' \
```
