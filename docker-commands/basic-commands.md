# Comandos básicos para se trabalhar com Docker.

## Docker Pull

### Comando usado para baixar uma imagem de um repositório de imagem e instalar no host.

```
docker pull <imagem>
```

## Docker Images

### Comando usado para listar imagens baixadas no host.

```
docker images
```

## Docker Images ls

### Comando para visualizar imagens baixadas no sistema.

```
docker images ls
```

## Docker rmi

### Comando usado para remover uma imagem baixada.

```
docker rmi <imagem>
```

## Docker run

### Comando usado para subir container.

```
docker run <imagem>
```

### Podemos deixar um processo rodando para que o container não seja encerrado após o run.. Use os parâmetros "-di":

```
docker run -id <imagem-a-ser-usada>
```

## Docker container ls / Docker ps

### Comando usado para listar containers ativos (também mostra o nome, ID, COMMAND entre outras informações).

```
docker container ls
```
### Ou

```
docker ps
```

## Docker container ls -a / Docker ps -a

### Comando para listar todos os container, mesmo os encerrados.

```
docker container ls -a
```

### Ou

```
docker ps -a
```

## Docker rm

### Comando para excluir containers.

```
docker rm <id do container>
```

## Docker stop

### Comando que encerra containers.

```
docker stop <id do container>
```

## Docker start

### Comando para iniciar um container encerrado.

```
docker start <id do container>
```

## Docker pause

### Comando que deixa o container parado, mas sem encerra-lo.

```
docker pause <id do container>
```

## Docker unpause

### Comando que "despausa" um container.

```
docker unpause <id do container>
```

## Docker exec

### Comando para executar comandos em um container.

```
docker exec <id do container> <comando>
```
### Exemplo (executando terminal bash em um container ubuntu):

```
docker exec -it <id do container> bash
```

<br>
<br>

# Mapeando portas

## Docker -p

### Com o comando "docker -p (minúsculo)" podemos especificar uma porta que queremos abrir do nosso host e qual porta do container irá receber o tráfego.

```
docker run -p porta-do-host-a-ser-aberta:porta-do-container-a-ser-exposta <imagem>
```

## Docker -P

### Com o P (maiúsculo) temos um efeito semelhante, porém ele escolhe as portas do host de forma aleatória.

```
docker run -d -P <imagem>
```

## Docker port

### Comando usado para verificar as portas em uso do container.

```
docker port <id do container>
```