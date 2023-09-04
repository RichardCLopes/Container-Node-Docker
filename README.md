# Container Node Docker

A seguir será apresentado o passo a passo de como criar um ambiente Node em  container Docker.

### Passo 1
Para criar o ambiente node é necessário ter baixado e instalado no computador o Docker, o Node e o Git. No momento que criei este repositório a versão atual do Docker é 24.0.5, a do Node é 20.5.1 e a do Git 2.41.0. Verifique as versões no seu computador rodando os comandos no terminal:
```
docker -v
node -v
git -v
```
### Passo 2
Clone este repositório dando um:
```
git clone <url_desse_repositório>
```
### Passo 3
Rode o comando abaixo para montar a imagem e construir o container:
```
docker build -t <nome_do_container> .
```
### Passo 4
Rode a aplicação dando um:
```
docker run -p 3000:3000 -d <nome_do_container> 
```
### Passo 5
Abra um navegador e digite na url localhost:3000 para ver a aplicação no ar.

### Passo 6
Para finalizar e parar a aplicação rode o comando abaixo para ver os containers em execução na sua máquina.
```
docker ps
```
Olhe o ID do container Node e rode o seguinte comando para dar um stop nela.
```
docker stop <id_container>.
```
