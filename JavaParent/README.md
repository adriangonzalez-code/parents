# java-parent

Parent POM base para proyectos Java con Spring Boot.

## Objetivo
Define la configuración principal y estándar para todos los proyectos derivados:
- Versiones de plugins y dependencias base.
- Configuración Maven global (Java 21, encoding, compilación).
- Gestión centralizada de BOMs (Spring Boot, Spring Cloud).

## ¿Cómo usarlo?
Haz que tus proyectos extiendan este POM en su `<parent>`:

```xml
<parent>
    <groupId>com.github.fernandocejas</groupId>
    <artifactId>java-parent</artifactId>
    <version>1.0.0-SNAPSHOT</version>
</parent>
```

Así garantizas consistencia en compilación y dependencias base.

---
## Notas
- No contiene dependencias directas, solo gestiona configuración global.
