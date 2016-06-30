# Principais comandos do Docker

1. Litar as imagens
```docker
docker images
```

2. Procurar imagens
```docker
docker search ubuntu
```

3. Puxar imagens
```docker
docker pull ubuntu
```

4. Remover imagens locais
```docker
docker rmi ID_ou_nome_da_imagem
```

5. Criar um container 
```docker
docker run nome_da_imagem
```

6. Criar um container e entrar no terminal
```docker
docker run -it nome_da_imagem /bin/bash
```

7. Criar um container com apelido
```docker
docker run --name apelido nome_da_imagem
```

8. Estado dos containers em atividade
```docker
docker ps
```

9. Estado de todos os containers
```docker
docker ps -a
```

10. Remove um container
```docker
docker rm id_ou_apelido
```

10. Outras informações do container
```docker
docker stats id_ou_apelido
```
Mais informações
```docker
docker inspect id_ou_apelido
```

11. Commitar alterações em uma imagem

As alterações que você faz em um container, durante sua execução, não são salvas, a menos que você gere uma nova imagem com base nesse container.

Para commitar o que você fez em uma imagem, utilize o comando commit:
Mais informações
```docker
docker commit ID/apelido nome_da_nova_imagem
```
Ele vai gerar uma nova imagem a partir desse commit.





