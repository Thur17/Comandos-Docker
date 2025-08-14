# Comandos-Docker

Comando para fazer o bulid do docker. 

```bash
docker compose build --no-cache
```

Rodar Docker sem travar Terminal 

```bash
docker compose up -d 
```

Acessar terminal de dentro do Docker com apache. 

```bash
docker exec -it nome-do-container-front bash
```
Acessar terminal de dentroo do Docker com Alpine.

```bash
docker exec -it nome-do-container-front sh
```
Após acessar rodar comando instalação de dependencias. 
```bash
composer install
```
Stop nos docker. 
```bash
docker compose down
```
Remover img do Docker.
```bash
docker rmi <nome-ou-id-da-imagem>
```
Remover todas as imagens, usar com moderação. 
```bash
docker rmi $(docker images -a -q)
```
Remover todas as imagens não usadas. 
```bash
docker image prune --all
```
