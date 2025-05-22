# Auth Service

O `auth-service` é responsável por autenticar usuários, registrar novas contas e validar tokens JWT.

Este microsserviço funciona como a **porta de entrada da plataforma**, gerando e validando tokens que são utilizados pelos demais serviços para garantir segurança e integridade das requisições.

---

## Funcionalidades principais

- Registro de novos usuários
- Autenticação com email e senha
- Geração de tokens JWT
- Validação de tokens e identificação de contas
