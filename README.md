# 🐳 Motores de Bases de Datos con Docker Compose

Este proyecto contiene varios archivos `docker-compose.yml` listos para levantar contenedores de los motores de bases de datos más utilizados. Todos están preparados para ser ejecutados con:

```bash
docker compose up -d
```

Cada archivo crea el entorno necesario para una base de datos específica. Ideal para pruebas, desarrollo local o estudios.

---

## 🔧 Requisitos

- Tener instalado Docker y Docker Compose.
- Funciona en cualquier distribución Linux.

---

## 📦 Bases de datos disponibles

Los archivos incluidos permiten levantar los siguientes motores:

- Oracle Database (`oracledb`)
- PostgreSQL (`postgresql`)
- SQL Server (`sqlserver`)
- MySQL (`mysql`) → Puerto 3306
- MariaDB (`mariadb`) → Puerto 3307 (evita conflicto con MySQL)
- Redis (`redis`)
- MongoDB (`mongodb`)

> ⚠️ Todos utilizan la imagen más reciente (`latest`).

---

## 🔐 Contraseñas y Usuarios

Todos los servicios utilizan una contraseña de ejemplo: `TuContraseña123`. **Recuerda cambiarla por una personalizada y segura**.

### Recomendaciones para contraseñas fuertes:

- Mínimo 8 caracteres
- Una mayúscula, una minúscula, un número y un símbolo

Ejemplo:

```text
Str0ng_P@ssw0rd2024
```

### Usuarios personalizados

En algunos archivos también se define un nombre de usuario por defecto. Puedes editarlo si lo deseas.

---

## 🚀 Uso rápido

1. Clona o descarga este repositorio.
2. Dirígete al directorio del motor que deseas levantar.
3. Ejecuta:

```bash
docker compose up -d
```

---

## 🧹 Apagar y eliminar contenedores

Para detener y borrar los contenedores:

```bash
docker compose down
```

---

## 📁 Organización

Cada archivo `docker-compose.yml` se encuentra en un subdirectorio con el nombre del motor correspondiente.

```
.
├── oracledb/
│   └── docker-compose.yml
├── postgresql/
│   └── docker-compose.yml
├── sqlserver/
│   └── docker-compose.yml
├── mysql/
│   └── docker-compose.yml
├── mariadb/
│   └── docker-compose.yml
├── redis/
│   └── docker-compose.yml
└── mongodb/
    └── docker-compose.yml
```

---

## 📝 Notas

- Oracle y SQL Server requieren contraseñas fuertes, de lo contrario el contenedor fallará al iniciar.
- Los puertos por defecto están expuestos y pueden modificarse según tus necesidades.

---

¡Listo para usar y experimentar con múltiples bases de datos en segundos! 🎉

