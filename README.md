
# 📦 curso-kubernetes

Este proyecto es un ejemplo de arquitectura de **microservicios con Spring Boot** y **Maven multimódulo**, listo para su despliegue en entornos como **Kubernetes** o **Docker Compose** (próximamente).

## 📁 Estructura del Proyecto

```
curso-kubernetes/
├── pom.xml                  # POM principal
├── msvc-usuarios/           # Microservicio de usuarios
│   └── pom.xml
├── msvc-cursos/             # Microservicio de cursos
│   └── pom.xml
```

Cada módulo es un microservicio independiente, pero comparten configuración común desde el POM padre.

---

## 🚀 Tecnologías Utilizadas

- Java 19 (puede migrarse fácilmente a 17 o 21)
- Spring Boot 3.5.0
- Maven multimódulo
- Spring Web / Spring Data

---

## ⚙️ Requisitos Previos

- [Java 19](https://jdk.java.net/19/) (o cambiar a 17/21)
- [Maven 3.8+](https://maven.apache.org/download.cgi)

---

## ▶️ Cómo Ejecutar el Proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/Danno1012/kubernete.git
cd kubernete
```

### 2. Compilar todo el proyecto

```bash
mvn clean install
```

### 3. Ejecutar un microservicio individual

```bash
cd msvc-usuarios
mvn spring-boot:run
```

O bien:

```bash
cd msvc-cursos
mvn spring-boot:run
```

---

## 🧪 Endpoints de prueba (ejemplo)

- `msvc-usuarios`: `http://localhost:8001/usuarios`
- `msvc-cursos`: `http://localhost:8002/cursos`

(Puertos y rutas pueden cambiar según configuración)

---

## 📌 Por hacer

- [ ] Dockerización de microservicios
- [ ] Despliegue en Kubernetes
- [ ] Agregar pruebas unitarias
- [ ] Integración con Eureka / Config Server
- [ ] Manejo de errores global
- [ ] Documentación Swagger/OpenAPI

---

## 👤 Autor

Daniel Flores  
[GitHub: Danno1012](https://github.com/Danno1012)
