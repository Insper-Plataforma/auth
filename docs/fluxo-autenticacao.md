# Fluxo de Autenticação

Este é o ciclo básico de autenticação e autorização do sistema:

## 1. Registro (`/auth/register`)

- O usuário envia seu nome, email e senha.
- O serviço cria a conta (em outro serviço) e retorna um token JWT.

## 2. Login (`/auth/login`)

- O usuário fornece email e senha.
- Se os dados estiverem corretos, um novo token é emitido.

## 3. Validação (`/auth/solve`)

- Um serviço interno envia o token para validação.
- O `auth-service` extrai o `idAccount` do token JWT e retorna.
