# Principais comandos do Docker

Litar as imagens
```docker
docker images
```

Procurar imagens
```docker
docker search ubuntu
```

Puxar imagens
```docker
docker pull ubuntu
```

Remover imagens locais
```docker
docker rmi ID_ou_nome_da_imagem
```

Criar um container 
```docker
docker run nome_da_imagem
```

Criar um container e entrar no terminal
```docker
docker run -it nome_da_imagem /bin/bash
```

Criar um container com apelido
```docker
docker run --name apelido nome_da_imagem
```

Estado dos containers em atividade
```docker
docker ps
```

Estado de todos os containers
```docker
docker ps -a
```

Remove um container
```docker
docker rm id_ou_apelido
```

Outras informações do container
```docker
docker stats id_ou_apelido
```
Mais informações
```docker
docker inspect id_ou_apelido
```

Commitar alterações em uma imagem

As alterações que você faz em um container, durante sua execução, não são salvas, a menos que você gere uma nova imagem com base nesse container.

Para commitar o que você fez em uma imagem, utilize o comando commit:
Mais informações
```docker
docker commit ID/apelido nome_da_nova_imagem
```
Ele vai gerar uma nova imagem a partir desse commit.





