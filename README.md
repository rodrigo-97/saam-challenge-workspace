# SAAM Auditoria - Workspace

## Passos para subir o projeto

### 1️⃣ Clonar os repositórios

**API**\
Abra o terminal na raiz do workspace e rode:

``` bash
git clone git@github.com:rodrigo-97/saam-challenge-api.git api
```

**Front-end**\
Ainda na raiz do workspace, rode:

``` bash
git clone git@github.com:rodrigo-97/saam-challenge-front-end.git front-end
```

### 2️⃣ Criar chaves pública e privada para geração do JWT

As chaves devem ser criadas dentro de `api/src/main/resources/`

**Chave privada**

``` bash
openssl genrsa -out api/src/main/resources/private.key 2048
```

**Chave pública**

``` bash
openssl rsa -in api/src/main/resources/private.key -pubout -out api/src/main/resources/public.key
```

### 3️⃣ Subir os containers

``` bash
docker compose up
```

### 4️⃣ Estrutura final esperada

```
workspace/
├── api/
└── front-end/

# Containers em execução:
saam-db
saam-api
saam-frontend
```

### 5️⃣ Acessando o sistema
- Front-end: http://localhost:5173/
- API (Swagger): http://localhost:8080/swagger-ui.html

O usuário padrão é
```
username = admin
password = admin
```