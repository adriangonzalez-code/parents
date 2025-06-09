# third-party-dependencies

Dependencias comunes de terceros para proyectos basados en Spring Boot.

## Objetivo
Centralizar y compartir dependencias usadas frecuentemente (Lombok, MapStruct, Apache Commons, Swagger/OpenAPI, testing) en todos los proyectos del ecosistema.

## Características
- Mantén versiones alineadas en todos los microservicios.
- Permite agregar/utilizar rápidamente herramientas externas validadas.

## ¿Cómo usarlo?
Inclúyelo en tu proyecto:

```xml
<dependency>
    <groupId>com.driagon</groupId>
    <artifactId>third-party-dependencies</artifactId>
    <version>1.0.0-SNAPSHOT</version>
    <type>pom</type>
    <scope>import</scope>
</dependency>
```
## Incluye

- Lombok para reducir boilerplate en código Java.
- MapStruct para mapeo de objetos.
- Apache Commons Lang para utilidades de Java, incluyendo manipulación de cadenas, números, fechas y más.
- Apache Common IO proporciona clases de utilidad, implementaciones de streams, filtros de archivos, comparadores de archivos, clases de transformación endian y mucho más.
- Apache Commons Collections para colecciones avanzadas y utilidades de manipulación de colecciones.
- Swagger/OpenAPI para documentación de APIs.
- Mockito para pruebas unitarias.
- AssertJ para aserciones más legibles.