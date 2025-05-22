# Setup e dependências 

Este módulo define apenas a **interface REST `AuthController`** e os DTOs relacionados.

---

## Requisitos

- Java 17+
- Lombok

---

## Como compilar

```bash
mvn clean install
```

---

## Dependências 

Requisitos no arquivo `pom.xml`:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-openfeign</artifactId>
</dependency>
```

---

## Como usar

Este módulo é usado como **dependência em `auth-service`**, que implementa de fato a interface.

Certifique-se de importar o pacote corretamente ao implementar:

```java
@RestController
public class AuthResource implements AuthController {
    // ...
}
```

---