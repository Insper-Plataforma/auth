# Endpoints da API

Base URL: `/auth`

---

## POST `/auth/register`

Registra um novo usuário e retorna o token JWT.

### Request Body
```json
{
  "name": "Ana Helena",
  "email": "ana@exemplo.com",
  "password": "12345678"
}
```

### Response
```json
{
    "token": "jwt.token.aqui"
}
```
---

## POST `/auth/login`

Registra um novo usuário e retorna o token JWT.

### Request Body
```json
{
  "email": "ana@exemplo.com",
  "password": "12345678"
}
```

### Response
```json
{
    "token": "jwt.token.aqui"
}
```

---

## POST `/auth/solve`

Resolve o token JWT e retorna o id da conta.

### Request
```json
{
  "token": "jwt.token.aqui"
}
``` 

### Response
```json
{
    "id": "uuid-da-conta"
}
```
---
