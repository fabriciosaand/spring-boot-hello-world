# Projeto Hello-World com Spring Boot

Este é um projeto simples "hello-world" utilizando Spring Boot, Java e Docker, criado com o objetivo de estudo.

## Tecnologias Utilizadas

- **Spring Boot** versão 3.2.5
- **Java** versão 21
- **Docker** para conteinerização

## Pré-requisitos

Antes de iniciar, certifique-se de ter instalado em sua máquina:

- Java 21
- Maven (para gerenciamento de dependências e build do projeto)
- Docker (para execução em contêineres)

## Executando o Projeto Localmente

Para executar o projeto localmente, siga estes passos:

1. Clone o repositório do projeto:

   ~~~shell
   git clone https://github.com/fabriciosaand/spring-boot-hello-world.git
   ~~~

2. Navegue até o diretório do projeto:

   ~~~shell
   cd spring-boot-hello-world 
   ~~~

3. Execute o projeto utilizando o Maven:

   ~~~shell
   ./mvnw spring-boot:run
   ~~~

   O aplicativo estará disponível em <http://localhost:8082>

## Executando o Projeto com Docker

Para executar o projeto utilizando Docker, siga estes passos:

1. Certifique-se de que a aplicação está parada. Digite `ctrl + c` no terminal para parar a aplicação.

2. Execute o comando para gerar arquivo **.jar**

   ~~~shell
   mvn clean package
   ~~~

3. Execute o contêiner utilizando o docker-compose

   ~~~shell
   docker-compose up -d
   ~~~

   Após esses passos, o aplicativo estará disponível em <http://localhost:8082>, assim como na execução local.

## Contribuições

Contribuições são sempre bem-vindas! Para contribuir, por favor, crie um fork do repositório, faça suas alterações e envie um pull request.
