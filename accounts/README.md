## Docker commands

### Criando o executável jar

- mvn clean install

### Executando a aplicação via terminal

- mvn spring-boot:run
- java -jar target/accounts-0.0.1-SNAPSHOT.jar

### Construindo a imagem

- docker build . -t renatoviana/accounts

### Construindo imagem via Buildpacks

- mvn spring-boot:build-image

### Adicionado tag na imagem

- docker image tag 3bfd renatobviana/accounts

### Removendo tag da imagem

- docker rmi renatoviana/accounts

### Inspecionar imagem criada

- docker image inspect 3bf

### Startando container

- docker run -p 8080:8080 -d renatobviana/accounts
- docker run -p 8081:8080 -d renatobviana/accounts

### Acessando container via terminal

- docker exec -it ca bash

### Parando container

- docker stop 0e

### Para o container instantaneamente

- docker kill 0e

### Pausando container

- docker container pause 0e

### Despausando container

- docker container unpause 0e

### Removendo container

- docker rm 0e

### Visualisando containers

- docker ps -a [-a retorna os containers parados]

### Inspecionar container

- docker container inspect de

### Docker logs

- docker logs -f de [-f atualiza para novos logs]

### Docker stats retorna informações sobre os containers rodando

- docker stats

### Docker push imagens

- docker push docker.io/renatobviana/accounts:latest

## Docker compose commands

### Start containers

- docker-compose up

### Stop containers

- docker-compose stop