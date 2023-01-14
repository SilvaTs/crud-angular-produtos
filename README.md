
<div align="center">
  <img alt="License" src="https://user-images.githubusercontent.com/47439833/212486728-fd9290a8-b2dd-40f5-bf54-96953d6bf0c0.png">
</div>

## 💻 Projeto
Objetivo desse projeto foi colocar os principais conceitos do angular em prática, consumindo uma api fake utilizando jason server.

---

## Como clonar o repositório

```
git clone https://github.com/SilvaTs/crud-angular-produtos.git
```
---
## Executando o projeto

**npm install** para instalar as dependências do projeto.
Em seguida, inicie o projeto.

---

```cl
ng s -o para executar o projeto front-end
json-server --watch db.json para executar api fake
```
# API FAKE COM JSON SERVER

- [API FAKE PRODUTOS](#api-fake-produto)
  - [Criar Produto](#criar-produto)
    - [Criar Produto Request](#criar-produto-request)
    - [Criar Produto Response](#criar-produto-response)
  - [Get Produto](#get-breakfast)
    - [Get Produto Request](#get-produto-request)
    - [Get Produto Response](#get-produto-response)
  - [Update Produto](#update-produto)
    - [Update Produto Request](#update-produto-request)
    - [Update Produto Response](#update-produto-response)
  - [Delete Produto](#delete-produto)
    - [Delete Produto Request](#delete-produto-request)
    - [Delete Produto Response](#delete-produto-response)

## Criar Produto

### Criar Produto Request

```js
POST /products
```

```json
    {
        "name": "caderno",
        "price": "75.90"
    }

```

### Criar Produto Response

```js
201 Created
```

```json
{
    "name": "caderno",
    "price": "75.90",
    "id": 7
}
```

## Get Produto

### Get Produto Request

```js
GET /products/{{id}}
```

### Get Produto Response

```js
200 Ok
```

```json
{
    "id": 3,
    "name": "Sansung S20+ Ultra",
    "price": "7520.89"
}
```

## Update Produto

### Update Produto Request

```js
PUT /products/{{id}}
```

```json
  {
    "id": 3,
    "name": "Sansung S20",
    "price": "7520.89"
  }
```

### Update Produto Response

```js
204 No Content
```

or

```js
201 Created
```

```yml
Location: {{host}}/Breakfasts/{{id}}
```

## Delete Breakfast

### Delete Produto Request

```js
DELETE /products/{{id}}
```

### Delete Produto Response

```js
204 No Content
```
