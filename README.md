# Fullcycle-3.0

# Link das Image no Docker Hub
Clique no nome do desafio para acessar a image no Docker Hub
-  [Image Desafio GO](https://hub.docker.com/repository/docker/esmaelfilho/fullcycle-go/general)
-  [Image Desafio Nginx com Node](https://hub.docker.com/repository/docker/esmaelfilho/fullcycle-go/general)


# Desafio GO

Esse desafio é muito empolgante principalmente se você nunca trabalhou com a linguagem Go!
Você terá que publicar uma imagem no docker hub. Quando executarmos:

docker run <seu-user>/fullcycle

Temos que ter o seguinte resultado: Full Cycle Rocks!!

Se você perceber, essa imagem apenas realiza um print da mensagem como resultado final, logo, vale a pena dar uma conferida no próprio site da Go Lang para aprender como fazer um "olá mundo".

Lembrando que a Go Lang possui imagens oficiais prontas, vale a pena consultar o Docker Hub.

3) A imagem de nosso projeto Go precisa ter menos de 2MB =)

Dica: No vídeo de introdução sobre o Docker quando falamos sobre o sistema de arquivos em camadas, apresento uma imagem "raiz", talvez seja uma boa utilizá-la.

Suba o projeto em um repositório Git remoto e coloque o link da imagem que subiu no Docker Hub.

Compartilhe o link do repositório do Git remoto para corrigirmos seu projeto.

#Resolução

## Build 

```
docker build -t esmaelfilho/fullcycle-go .
```

## RUN

```
docker run --rm esmaelfilho/fullcycle-go
```

## PULL
```
docker pull esmaelfilho/fullcycle-go
```

## Link Image no DockerHub
-  [GO]([https://pages.github.com/](https://hub.docker.com/repository/docker/esmaelfilho/fullcycle-go/general))
-  [Nginx com Node]([https://pages.github.com/](https://hub.docker.com/repository/docker/esmaelfilho/fullcycle-go/general))





# Desafio Nginx com Node.js

Nesse desafio você colocará em prática o que aprendemos em relação a utilização do nginx como proxy reverso. A idéia principal é que quando um usuário acesse o nginx, o mesmo fará uma chamada em nossa aplicação node.js. Essa aplicação por sua vez adicionará um registro em nosso banco de dados mysql, cadastrando um nome na tabela people.

O retorno da aplicação node.js para o nginx deverá ser:

<h1>Full Cycle Rocks!</h1>

- Lista de nomes cadastrada no banco de dados.

Gere o docker-compose de uma forma que basta apenas rodarmos: docker-compose up -d que tudo deverá estar funcionando e disponível na porta: 8080.

Suba tudo em um repositório e faça a entrega.

* A linguagem de programação para este desafio é Node/JavaScript.
