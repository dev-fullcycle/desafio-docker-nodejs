# Desafio Docker Nodejs
Desafio proposto pelo Wesley para manipulação de dockers e desenvolvimento local  
dentro do container montar A idéia principal é que quando um usuário acesse o  
nginx, o mesmo fará uma chamada em nossa aplicação node.js. Essa aplicação por  
sua vez adicionará um registro em nosso banco de dados mysql, cadastrando um nome na tabela people.

O retorno da aplicação node.js para o nginx deverá ser:
<h1>Full Cycle Rocks!</h1>

- [ ] Lista de nomes cadastrada no banco de dados.

Gere o docker-compose de uma forma que basta apenas rodarmos: 
docker-compose up -d que tudo deverá estar funcionando e disponível na porta: 8080.

Suba tudo em um repositório e faça a entrega.

* A linguagem de programação para este desafio é Node/JavaScript.

## Repositorio das imagens docker no dockerhub pacalexandre
```resultado```
- https://hub.docker.com/r/pacalexandre/

## Documentação Nodejs.
-

## Versões instaladas em meu ambiente.
```bash 
NAME="Linux Mint"
VERSION="21.1 (Vera)"
ID=linuxmint
ID_LIKE="ubuntu debian"
PRETTY_NAME="Linux Mint 21.1"
VERSION_ID="21.1"
HOME_URL="https://www.linuxmint.com/"
SUPPORT_URL="https://forums.linuxmint.com/"
BUG_REPORT_URL="http://linuxmint-troubleshooting-guide.readthedocs.io/en/latest/"
PRIVACY_POLICY_URL="https://www.linuxmint.com/"
VERSION_CODENAME=vera
UBUNTU_CODENAME=jammy

Docker version 24.0.5, build ced0996
Docker Compose version v2.20.2
```
## Comando utilizados.

```bash
#No terminal para subior projeto parar editar em go 
docker compose up --build -d

docker build -t pacalexandre/fullcycle -f Dockerfile.desafio .

docker login

docker push pacalexandre/fullcycle

docker rm $(docker ps -a -q )

```