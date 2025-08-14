
# 🐳 Comandos Docker

Guia rápido de comandos Docker úteis para desenvolvimento.

---

## 🚀 Build do Docker

Criar a imagem do Docker sem usar cache:

```bash
docker compose build --no-cache
```

---

## ⚡ Rodar Docker em background

Executa o Docker sem travar o terminal:

```bash
docker compose up -d
```

---

## 🖥️ Acessar terminal do container

### Apache
```bash
docker exec -it nome-do-container-front bash
```

### Alpine
```bash
docker exec -it nome-do-container-front sh
```

---

## 📦 Instalar dependências

Após acessar o terminal do container, instalar dependências do projeto:

```bash
composer install
```

---

## 🛑 Parar containers

```bash
docker compose down
```

---

## 🗑️ Remover imagens Docker

### Remover uma imagem específica
```bash
docker rmi <nome-ou-id-da-imagem>
```

### Remover todas as imagens (use com cuidado!)
```bash
docker rmi $(docker images -a -q)
```

### Remover todas as imagens não usadas
```bash
docker image prune --all
```