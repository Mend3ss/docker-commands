# Comandos básicos para se trabalhar com Docker.

## Docker Pull

### Comando usado para baixar uma imagem de um repositório de imagem e instalar no host.

```
docker pull <imagem>
```

## Docker Images

### Comando usado para listar imagens baixadas no host

```
docker images
```

## Docker Images ls

### Comando para visualizar imagens baixadas no sistema

```
docker images ls
```

## Docker rmi

### Comando usado para remover uma imagem baixada

```
docker rmi <imagem>
```

## Docker run

### Comando usado para subir container

```
docker run <imagem>
```

## Docker container ls / Docker ps

### Comando usado para listar containers ativos (também mostra o nome, ID, COMMAND entre outras informações)

```
docker container ls
```
### Ou

```
docker ps
```

## Docker container ls -a / Docker ps -a

### comando para listar todos os container, mesmo os encerrados.

```
docker container ls -a
```

### Ou

```
docker ps -a
```

## Docker rm

### comando para excluir containers

```
docker rm <id do container>
```