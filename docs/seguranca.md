# Segurança

O Auth Service é responsável por gerar, validar e decodificar tokens JWT.

## Funcionamento

1. O usuário faz login ou se registra.
2. Um token JWT é gerado e retornado (`TokenOut`).
3. Esse token é usado nos demais serviços para autenticação.

---

## Benefícios do JWT

- Sem necessidade de sessão no servidor
- Escalável e stateless
- Informações como `idAccount` ficam disponíveis no payload

---

## Endpoint de Verificação

O endpoint `/auth/solve` serve para verificar a autenticidade do token e obter o `idAccount` associado.

---

## Observações

- O token deve ser tratado com confidencialidade
- Recomenda-se uso via header: `Authorization: Bearer <token>`

---