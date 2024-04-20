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

1. Certifique-se que a aplicação está parada.

2. Execute o comando para gerar arquivo **.jar**

   ~~~shell
   mvn clean package
   ~~~

3. Execute o contêiner utilizando o docker-compose

   ~~~shell
   docker compose up -d
   ~~~

   Após esses passos, o aplicativo estará disponível em <http://localhost:8082>, assim como na execução local.

## Parando o Contêiner Docker

Se você precisar parar o contêiner Docker que está executando o aplicativo Spring Boot, você pode usar o seguinte comando:

~~~shell
docker compose down
~~~

## Parando a Aplicação Localmente

Quando a aplicação estiver sendo executada localmente através do Maven, você pode pará-la pressionando:

- **Ctrl+C** no terminal se estiver rodando em modo interativo.

Ou, se você iniciou a aplicação em segundo plano, você pode pará-la encontrando o ID do processo e utilizando o comando `kill`:

1. Encontre o ID do processo com:

   ~~~shell
   ps -f | grep java
   ~~~

2. Pare a aplicação com:

   ~~~shell
   kill [PID]
   ~~~

   Substitua [PID] pelo número do ID do processo que você deseja parar.

## Contribuições

Contribuições são sempre bem-vindas! Para contribuir, por favor, crie um fork do repositório, faça suas alterações e envie um pull request.
