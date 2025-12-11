
# SAAM Auditoria - Workspace

## Tecnologias utilizadas

- **Back-end:** Java, Spring Boot, PostgreSQL
- **Front-end:** ReactJS com Vite.js

## Passos para subir o projeto

### Passo 1: Clonar os repositórios

Abra o terminal no local onde deseja clonar o workspace e rode:

```bash
git clone git@github.com:rodrigo-97/saam-challenge-workspace.git
```

Entre na pasta do workspace:

```bash
cd saam-challenge-workspace
```

**Clonar API**

```bash
git clone git@github.com:rodrigo-97/saam-challenge-api.git api
```

**Clonar Front-end**

```bash
git clone git@github.com:rodrigo-97/saam-challenge-front-end.git front-end
```

### Passo 2: Gerar chaves pública e privada para JWT

As chaves devem ser criadas dentro de `api/src/main/resources/`.

**Chave privada:**

```bash
openssl genrsa -out api/src/main/resources/private.key 2048
```

**Chave pública:**

```bash
openssl rsa -in api/src/main/resources/private.key -pubout -out api/src/main/resources/public.key
```

### Passo 3: Subir os containers

```bash
docker compose up
```

### Passo 4: Estrutura final esperada

```
workspace/
├── api/
└── front-end/

# Containers em execução:
saam-db
saam-api
saam-frontend
```

### Passo 5: Acessando o sistema

- **Front-end:** [http://localhost:5173/](http://localhost:5173/)  
- **API (Swagger):** [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

### Passo 6: Usuário padrão

```
username: admin
password: adminadmin
```
