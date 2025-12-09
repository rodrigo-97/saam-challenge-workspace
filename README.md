# SAAM Auditoria - Workspace

## Passos para subir o projeto

### 1️⃣ Clonar os repositórios

**API**
Abra o terminal na raíz do projeto e rode:

```bash
git clone git@github.com:rodrigo-97/saam-challenge-api.git api
```

Isso vai criar uma pasta com todo o código da `api`

**Front-end**
No mesmo diretório, rode:

```bash
git clone git@github.com:rodrigo-97/saam-challenge-front-end.git front-end
```
Isso vai criar uma pasta com todo o código do `front-end`


### 2️⃣ Subir os containers
```bash
docker-compose up
```

### 3️⃣ Estrutura final esperada

Após rodar tudo, você terá:
```
workspace/
├── api/            # Código da API
└── front-end/      # Código do Front-end

Containers em execução:
- saam-db
- saam-api
- saam-frontend
```

### 4️⃣ Acessando o sistema
- **Front-end:** http://localhost:5173
- **Api:** http://localhost:8080/swagger-ui
