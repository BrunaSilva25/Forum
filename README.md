# Forum

Este é um projeto desenvolvido como parte do desafio do programa ONE da Alura, com o objetivo de criar uma plataforma de fórum.
O Forum Hub é uma aplicação de fórum desenvolvida com Spring Boot, que permite aos usuários criar tópicos, fazer perguntas e fornecer respostas.

## Funcionalidades

- **Tópicos:** Os usuários podem visualizar, criar e pesquisar tópicos de interesse.
- **Perguntas e Respostas:** Cada tópico pode ter várias perguntas e respostas associadas.
- **Validação de Dados:** Utilização de validação de dados utilizando anotações do Jakarta Bean Validation.
- **Segurança:** Autenticação de usuários utilizando Spring Security e geração de tokens JWT.
- **Documentação da API:** Utilização do Springdoc OpenAPI para documentação automática da API.

## Tecnologias Utilizadas

- Java 17
- Spring Boot 3.3.1
- PostgreSQL (banco de dados)
- Lombok (para redução de código boilerplate)
- Spring Data JPA (para persistência de dados)
- Spring Security (para segurança da aplicação)
- Spring Validation (para validação de dados)
- Auth0 Java JWT (para manipulação de tokens JWT)
- Springdoc OpenAPI (para documentação da API)

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- **Model:** Contém as entidades de dados como `Usuario`, `Topico`, `Resposta`, etc.
- **Repository:** Interfaces que estendem `JpaRepository` para acesso aos dados.
- **Service:** Camada de serviço que implementa regras de negócio.
- **Controller:** Controllers que lidam com requisições HTTP e respondem com dados.
- **Exceptions:** Classes para tratamento de exceções.
- **Configurações:** Configurações adicionais da aplicação.

## Como Executar

1. **Pré-requisitos:**
   - Java JDK 17 ou superior instalado.
   - PostgreSQL instalado e configurado.

2. **Configuração do Banco de Dados:**
   - Crie um banco de dados PostgreSQL chamado `forumhub`.
   - Configure as credenciais do banco no arquivo `application.properties`.

3. **Execução:**
   - Clone o repositório.
   - Navegue até o diretório do projeto.
   - Execute `mvn spring-boot:run` para iniciar a aplicação.

4. **Acesso à API:**
   - Acesse `http://localhost:8080/swagger-ui.html` para visualizar a documentação da API.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para enviar pull requests e relatar problemas.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
