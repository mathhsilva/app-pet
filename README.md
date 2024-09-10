  

# API de Gerenciamento de Produtos Pet 🐾

  

## Descrição

Este projeto é uma API RESTful desenvolvida em Java com Spring Boot para o gerenciamento de produtos de uma loja online de pets. A API oferece operações de **CRUD** (Criar, Ler, Atualizar, Excluir) e possibilita a manipulação de informações como nome, descrição, preço, categoria e quantidade em estoque de produtos, com regras de negócio que garantem a integridade dos dados.

  

## Funcionalidades

  

-  **Criar Produto**: Adicionar novos produtos com as seguintes informações:

- Nome

- Descrição

- Preço

- Categoria (ração, brinquedo, acessórios, medicamentos)

- Quantidade em estoque

-  **Consultar Produtos**:

- Listar todos os produtos

- Buscar um produto específico pelo seu ID

-  **Atualizar Produto**: Atualizar informações como nome, preço, quantidade, etc.

-  **Excluir Produto**: Remover um produto do sistema através do ID.

  

## Tecnologias Utilizadas

  

-  **Java 11** ou superior

-  **Spring Boot 2.5** ou superior

-  **Banco de Dados SQL**: H2 (para testes), PostgreSQL ou MySQL

-  **JUnit** e **Mockito** para testes unitários

-  **Swagger/OpenAPI** para documentação da API

-  **Git** e **GitHub** para controle de versão

  

## Regras de Negócio

  

- O preço do produto não pode ser negativo.

- A categoria do produto deve ser uma das seguintes: `ração`, `brinquedo`, `acessórios`, `medicamentos`.

  

## Como Executar o Projeto

  

1. Clone o repositório:

```bash

git clone https://github.com/seu-usuario/pet-products-api.git

```

2. Acesse o diretório do projeto:

```bash

cd pet-products-api

```

3. Compile e rode o projeto:

```bash

./mvnw spring-boot:run

```

4. A API estará disponível em:

```

http://localhost:8080/api/produtos

```

  

## Endpoints

  

| Método | Endpoint | Descrição |

|--------|-------------------------|-----------------------------------|

| GET | `/api/produtos` | Listar todos os produtos |

| GET | `/api/produtos/{id}` | Obter detalhes de um produto |

| POST | `/api/produtos` | Criar um novo produto |

| PUT | `/api/produtos/{id}` | Atualizar informações de um produto |

| DELETE | `/api/produtos/{id}` | Remover um produto |

  

## Banco de Dados

  

Para facilitar o desenvolvimento, o banco de dados H2 será utilizado no ambiente de teste. Para produção, é recomendado utilizar PostgreSQL ou MySQL. A configuração do banco de dados pode ser feita no arquivo `application.properties` ou `application.yml`.

  

## Testes

  

Os testes unitários foram implementados utilizando **JUnit** e **Mockito** para garantir que os endpoints da API funcionem corretamente. Para rodar os testes, utilize:

  

```bash

./mvnw  test

```

  

## Documentação da API

  

A documentação da API foi gerada utilizando **Swagger/OpenAPI**. Para acessar a interface do Swagger, execute o projeto e acesse:

  

```

http://localhost:8080/swagger-ui.html

```

  

## Deploy (Opcional)

  

Se desejar realizar o deploy da aplicação, é possível utilizar serviços gratuitos como **Heroku** ou **Render**.

  

## Melhorias Futuras

  

- Adicionar integração com MongoDB para armazenar revisões e classificações de clientes.

- Implementar autenticação e autorização nos endpoints.

- Fazer o deploy em um ambiente de produção.

  

---

  

**Autor**: [Matheus Silva](https://github.com/mathhsilva)
