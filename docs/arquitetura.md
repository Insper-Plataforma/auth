# Arquitetura do Auth Service

O serviço segue a estrutura típica de microsserviços com Spring Boot.

## Estrutura de Pastas

```bash
src/main/java/store/auth/
├── AuthController.java # Interface REST com os endpoints
├── LoginIn.java # DTO de entrada para login
├── RegisterIn.java # DTO de entrada para registro
├── SolveOut.java # DTO de saída com id da conta
├── TokenOut.java # DTO de saída com token JWT
```

---

## Tecnologias utilizadas

- Java 17+
- Spring Boot
- JWT (para geração e verificação de tokens)
- Lombok (para reduzir boilerplate)
