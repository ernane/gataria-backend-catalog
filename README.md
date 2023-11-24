# Gataria Backend Catalog

Variáveis de ambiente necessárias:
- MONGO_DATABASE
- MONGO_URL

Exemplo:

```
export MONGO_URL="mongodb+srv://USER:PASSWORD@exampleUrl.mongodb.net/"
export MONGO_DATABASE="dev"
```

Iniciando o backend

```
npm start
```

Para rodar os testes

```
npm test
```

# Execução local com Docker

```bash
docker run --name gataria-backend-catalog \
-e MONGO_DATABASE=$MONGO_DATABASE \
-e MONGO_URL=$MONGO_URL \
-p 3010:3010 \
-d gataria-backend-catalog:dev2
```