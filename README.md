## Docker & Kubernetes

+ Containers são criados a partir de imagens
+ Podemos ter vários containers de uma unica imagem

Para ter acesso ao terminal do container:

```zsh
docker exec -it <container_name>
```

+ **CMD**: roda sempre quando um container inicia
 

+ **RUN**: roda quando cria a imagem

Para criar uma imagem a partir de um dockerfile:
 
```zsh
docker build .
```

Padrão de portas:
```
<PORTA EXTERNA>:<PORTA INTERNA DO CONTAINER>
```

Para criar um novo container:
```zsh
docker run <nome_imagem>
```

Listar todos os containers parados:
```zsh
docker ps -a
```

Vincular o terminal com um determinado container:
```zsh
docker attach <nome_container>
```

Para destacar:
```zsh
docker start -d <container>
```

Abrir os logs de um container e manter imprimindo no terminal:
```zsh
docker logs -f <container_ID>
```
