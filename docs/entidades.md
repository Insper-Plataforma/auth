# Entidades

## LoginIn

DTO de entrada para autenticação de usuários.

Campos:
- `email`: email do usuário
- `password`: senha em texto puro

---

## RegisterIn

DTO de entrada para registrar um novo usuário.

Campos:
- `name`: nome do usuário
- `email`: email do usuário
- `password`: senha do usuário

---

## TokenOut

DTO de saída que representa o token JWT emitido após login ou registro.

Campos:
- `token`: string com o JWT gerado

---

## SolveOut

DTO de saída usado para extrair informações do token enviado.

Campos:
- `idAccount`: identificador da conta associado ao token
---