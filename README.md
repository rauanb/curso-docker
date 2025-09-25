# Curso Docker
Anotações do curso de docker do Matheus Muller

## 1 - Introdução do Docker
* **Otimização:** Compartilha Kernel com o Host
* **Empacotamento:** contém todas as dependências
* **Imutablidade:** baseado em imagem pré-definida com as dependências

## 2 - Comandos
### Imagens
**docker image**
* **ls:** lista as imagens **~>** **docker images**
* **inspect imagem:tag:** mostra o conteúdo da imagem

**docker pull**
* **imagem:** download da tag latest **~>** NÃO RECOMENDADO
* **imagem:tag_específica:** download da tag específica
    * `docker pull nginx:1.21.6-alpine`

### Containers
**docker run**

* **-d imagem:tag:** roda um container da imagem em background
* **-P:** expõe a porta aleatória
* **-p PORTA_HOST:PORTA_CONT:** expõe a porta especificada

**docker ps**
* lista os containers em execução
* **-a:** lista todos os containers, mesmo os parados

**docker logs ID_ou_NOME**
* mostra os logs do container
* **-f:** mostra os logs do container em tempo real

**docker inspect ID**
* mostra o conteúdo do container (mesmo de um ID parado)

**docker stats**
* mostra uso de recursos do host pelos containers
* **ID:** mostra o uso somente do container