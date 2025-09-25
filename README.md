# Curso Docker
Anotações do curso de docker do Matheus Muller

## 1 - Introdução do Docker
* **Otimização:** Compartilha Kernel com o Host
* **Empacotamento:** contém todas as dependências
* **Imutablidade:** baseado em imagem pré-definida com as dependências

## 2 - Comandos
### Imagens
* **docker image ls:** lista as imagens
* **docker images:** abreviação do ls
* **docker pull imgem:** download da tag latest **~>** NÃO RECOMENDADO
* **docker pull imagem:tag_específica:** download da tag específica
    * `docker pull nginx:1.21.6-alpine`
* **docker image inspect imagem:tag:** mostra o conteúdo da imagem

### Containers
* **docker container run -d imagem:tag:** roda um container da imagem em background
* **docker run -d imagem:tag:** abreviação do camando anterior
* **docker container ls:** lista os containers em execução
* **docker ps:** abreviação do comando anterior
* **docker ps -a:** lista todos os containers, mesmo os parados
* **docker inspect ID:** mostra o conteúdo do container (mesmo de um ID parado)