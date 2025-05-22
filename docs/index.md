# Auth Interface

Este módulo define a **interface Feign** para comunicação com o microsserviço `auth-service`, responsável pela autenticação e autorização de usuários.

---

## Objetivo

Facilitar a comunicação entre microsserviços por meio de chamadas REST encapsuladas, utilizando Feign Client, evitando duplicação de lógica HTTP.

---

## Pacote

- `store.auth` - Pacote principal que contém a interface Feign e os objetos de entrada e saída.

---

## Estrutura dos arquivos

| Arquivo               | Descrição                                                                     |
| --------------------- | ----------------------------------------------------------------------------- |
| `AuthController.java` | Interface Feign com os endpoints disponíveis do microsserviço de autenticação |
| `LoginIn.java`        | Objeto de entrada para o login na conta                                       |
| `RegisterIn.java`     | Objeto de entrada para o registro da conta                                    |
| `SolveOut.java`       | Id da conta que é retornado quando realiza o registro                         |
| `TokenOut.java`       | Token da conta que é retornado quando realiza o login                         |
