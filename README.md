# <p align = "center"> Prática Docker </p>

<p align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png"/>
</p>

<p align = "center">
   <img src="https://img.shields.io/badge/author-Januacele Vieira-4dae71?style=flat-square" />
   <img src="https://img.shields.io/badge/author-Docker-4dae71?style=flat-square" />
</p>

##  :clipboard: Descrição
  Projeto para exercitar a criação de uma imagem node utilizando o docker. O projeto foi desenvolvido em typeScript e seu objetivo é escolher um nome
  aleatório a partir de uma lista randomizada. 
***
## :computer:	 Tecnologias e Conceitos

-<img align="left" alt="Node.js" width="30px" src="https://cdn.iconscout.com/icon/free/png-256/node-js-3628954-3030179.png" />
-<img align="left" alt="TypeScript" width="30px" src="https://cdn.icon-icons.com/icons2/2107/PNG/512/file_type_typescript_icon_130108.png" />
-<img align="left" alt="Prisma" width="30px" src="https://d2eip9sf3oo6c2.cloudfront.net/tags/images/000/001/287/square_480/prismaHD.png" />
-<img align="left" alt="Docker" width="30px" src="https://www.docker.com/wp-content/uploads/2022/05/Docker_Temporary_Image_Google_Blue_1080x1080_v1.png" />

***
## :rocket: Rotas

```yml
POST /students
    - Rota para cadastrar um novo estudante
    - headers: {}
    - body:
        {
        "students": [
          {"name": "Davi"}
          ]
        }

```

```yml
GET /students
    - Rota para listar todos os nomes de estudantes cadastrados
    - headers: {}
    - body:{}
       
```

```yml
GET /students/random 
    - Rota para sortear o nome de um estudante de forma aleatória
    - headers: { "Authorization": "Bearer $token" }
    - body: {}
``` 

## 🏁 Rodando a aplicação

Este projeto foi inicializado usando a imagem do node.js via docker, logo garanta que você possui o docker instalado em sua máquina.
-link intalação docker: https://docs.docker.com/get-docker/

Primeiro, faça o clone desse repositório na sua maquina:

```
git clone https://github.com/Januacele/docker-exercises
```

Depois, dentro da pasta, rode o seguinte comando para instalar as dependencias.

```
npm install
```

Finalizado o processo, é só buildar e inicializar o servidor:

```
docker-compose up --build
```
Após o build pode inicializar o servidor com o comando:

```
docker-compose up
```
:stop_sign: Esse projeto não possui interface front-end, fique a vontade para implementar. 
