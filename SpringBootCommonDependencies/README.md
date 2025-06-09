# spring-boot-dependencies

Dependencias Spring Boot mínimas y estándar para levantar microservicios REST.

## Objetivo
Facilitar la creación de servicios rápidos, homogéneos y productivos, minimizando configuración y asegurando buenas prácticas de arranque.

## Incluye
- Starter web, actuator y validaciones.
- Starter para Log4j2 (logging centralizado).
- Starter test para pruebas unitarias.
- [Opcional] Starter de logging por defecto excluido para evitar conflictos.

## ¿Cómo usarlo?
Inclúyelo en tu proyecto:

```xml
<dependency>
    <groupId>com.driagon</groupId>
    <artifactId>spring-boot-dependencies</artifactId>
    <version>1.0.0-SNAPSHOT</version>
    <type>pom</type>
    <scope>import</scope>
</dependency>
```

---

## Extensión y recomendaciones
- Si necesitas más starters (JPA, Security, Messaging), puedes agregarlos como módulos aparte o en este mismo BOM.
- Se recomienda estandarizar el patrón y formato de logs; pero puedes personalizarlo según las guías.

---

## Soporte
Para agregar nuevas dependencias, sugiere el cambio al equipo central.

## Dependencias
- Spring Boot Starter Web
- Spring Boot Starter Actuator
- Spring Boot Starter Validation
- Spring Boot Starter Log4j2
- Spring Boot Starter Logging (opcional, excluido por defecto)
- Spring Boot Starter AOP
- Spring Cloud Starter OpenFeign
- Spring Cloud Starter Bootstrap
- Spring Boot Starter Test
