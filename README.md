# Maven Dependency Architecture

## Overview

This repository defines a dependency architecture for Java projects based on Spring Boot and Spring Cloud, using a parent POM (`java-parent`) and several common dependency modules to facilitate management and reuse in REST APIs.

---

## Main Modules

### 1. java-parent

- **Type:** Parent POM
- **Purpose:** Centralizes configuration of versions, plugins, and common dependencies.
- **Includes:**
    - Versions for Java, Spring Boot, Spring Cloud, MapStruct, Lombok, Jacoco, Jasypt, among others.
    - Management of build, packaging, and code analysis plugins.
    - Import of Spring Boot and Spring Cloud BOMs.
    - Exclusion of `spring-boot-starter-logging` to allow custom logging.

---

### 2. spring-boot-common-dependencies

- **Type:** POM
- **Purpose:** Groups native Spring Boot and Spring Cloud starters and dependencies.
- **Includes:**
    - `spring-boot-starter`, `spring-boot-starter-web`, `spring-boot-starter-log4j2`, `spring-boot-starter-aop`
    - Spring Cloud starters such as `openfeign` and `bootstrap`
    - Micrometer for tracing

---

### 3. third-party-dependencies

- **Type:** POM
- **Purpose:** Centralizes common third-party dependencies.
- **Includes:**
    - Apache Commons (`commons-lang3`, `commons-collections4`, `commons-io`)
    - Swagger/OpenAPI (`springdoc-openapi-starter-webmvc-ui`)

---

### 4. spring-boot-testing-dependencies

- **Type:** POM
- **Purpose:** Provides dependencies for testing in Spring Boot projects.
- **Includes:**
    - `spring-boot-starter-test`
    - `spring-security-test`
    - `assertj-core`

---

## Architecture Advantages

- **Centralization of versions and dependencies** to avoid conflicts and ease updates.
- **Reuse** of configurations and dependencies across multiple projects.
- **Ease of maintenance** and scalability for development teams.

---

## Created by

![Logo Driagon.png](Logo%20Driagon.png)