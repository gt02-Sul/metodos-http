# Aula sobre métodos HTTP na prática

*Material Complementar - Consumo de API*\
Nesta aula prática usamos o insomnia para ganhar habilidade em requisições ao endpoint ( gt/api/users ) de uma mockAPI. \
<br>

### Realizamos operações usando os principais métodos:
**GET: Recuperar todos os usuários**
```
curl -X GET https://668dcca8bf9912d4c92be825.mockapi.io/gt/api/users
```

**GET: Recuperar usuário por id**
```
curl -X GET https://668dcca8bf9912d4c92be825.mockapi.io/gt/api/users/1
```

**POST: Adicionar um novo usuário**
```
curl -X POST https://668dcca8bf9912d4c92be825.mockapi.io/gt/api/users -H "Content-Type: application/json" -d '{"name": "Carlos Segundo", "avatar": "https://cloudflare-ipfs.com/ipfs/Qmd3W5DuhgHirLHGVixi6V76LhCkZUz6pnFt5AJBiyvHye/avatar/572.jpg"}'

```

**PUT: Atualizar um usuário existente (substituição completa)**
```
curl -X PUT https://668dcca8bf9912d4c92be825.mockapi.io/gt/api/users/1 -H "Content-Type: application/json" -d '{"name": "Carlos Primeiro", "avatar": "https://cloudflare-ipfs.com/ipfs/Qmd3W5DuhgHirLHGVixi6V76LhCkZUz6pnFt5AJBiyvHye/avatar/572.jpg"}'

```

**DELETE: Deletar um produto existente**
```
curl -X DELETE https://668dcca8bf9912d4c92be825.mockapi.io/gt/api/users/1

```
