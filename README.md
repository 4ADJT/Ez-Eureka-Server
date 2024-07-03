# Ez-Blue - The Blue Zone Easy
## Ez-Eureka-Server

Ez-Eureka-Server é um serviço de descoberta baseado no Netflix Eureka, que permite que outros microserviços descubram e se comuniquem entre si sem a necessidade de configuração manual de endpoints.

## Intenção

O objetivo deste serviço é atuar como um registro central para todos os microserviços da aplicação, facilitando a descoberta de serviços e o balanceamento de carga.

## Como executar

### Requisitos

- JDK 17+
- Maven 3.6.3+
- Docker (opcional para execução com Docker)

## Executar localmente

1. Clone o repositório:
```sh
git clone https://github.com/4ADJT/Ez-Eureka-Server.git
cd Ez-Eureka-Server
```

2. Compile e execute o projeto
```sh
mvn clean package
mvn spring-boot:run
```
## Executar com Docker

1. Compile o projeto e crie a imagem Docker:
```sh
docker build -t ez-eureka-server .
```

2. Execute o container:
```sh
docker run -p 8761:8761 ez-eureka-server
```

## Configuração
A configuração do Ez-Eureka-Server pode ser encontrada no arquivo application.properties na pasta src/main/resources.