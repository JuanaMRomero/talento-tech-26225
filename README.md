# FakeStore API - CRUD desde Node.js

## Descripción del proyecto

Este proyecto consiste en una aplicación de consola desarrollada con **Node.js** que permite realizar operaciones básicas sobre productos mediante el consumo de la API REST de [FakeStore API](https://fakestoreapi.com/).

La aplicación recibe comandos desde la terminal utilizando `process.argv` y ejecuta diferentes solicitudes HTTP para consultar, crear y eliminar productos.

El objetivo es poner en práctica conceptos fundamentales de Node.js, consumo de APIs, programación asíncrona y manejo de solicitudes HTTP.

## Tecnologías utilizadas

- **Node.js:** entorno de ejecución de JavaScript.
- **JavaScript (ES Modules):** desarrollo de la lógica de la aplicación.
- **Fetch API:** realización de solicitudes HTTP.
- **FakeStore API:** API REST utilizada para gestionar los productos.
- **Terminal:** ejecución de comandos mediante argumentos.

## Funcionalidades

La aplicación permite realizar las siguientes operaciones:

| Método HTTP | Funcionalidad | Descripción |
|---|---|---|
| GET | Consultar productos | Obtiene el listado de productos o consulta un producto específico. |
| POST | Crear productos | Envía un nuevo producto con título, precio y categoría. |
| DELETE | Eliminar productos | Realiza una solicitud para eliminar un producto mediante su ID. |

## Estructura del proyecto

```text
fake-store-api/
│
├── index.js
├── package.json
└── README.md
```

## Instalación y configuración

### 1. Clonar el repositorio

```bash
git clone URL_DEL_REPOSITORIO
```

### 2. Ingresar a la carpeta

```bash
cd fake-store-api
```

### 3. Instalar dependencias

El proyecto utiliza funcionalidades nativas de Node.js, por lo que no requiere dependencias externas.

### 4. Ejecutar la aplicación

Los comandos se ejecutan desde la terminal utilizando:

```bash
node index.js COMANDO PARAMETROS
```

## Ejemplos de uso

### GET - Consultar productos

Obtener todos los productos:

```bash
node index.js GET products
```

Consultar productos de una categoría:

```bash
node index.js GET products/category/electronics
```

Consultar un producto específico:

```bash
node index.js GET products/1
```

### POST - Crear un producto

Crear un producto indicando título, precio y categoría:

```bash
node index.js POST products "Notebook Lenovo" 850000 electronics
```

El programa envía los datos mediante una solicitud POST y muestra la respuesta de la API, incluyendo el ID del producto creado.

### DELETE - Eliminar un producto

Eliminar un producto indicando su ID:

```bash
node index.js DELETE products/1
```

El programa realiza una solicitud DELETE y muestra la respuesta recibida.

## Conceptos aplicados

Durante el desarrollo se trabajaron los siguientes conceptos:

- Uso de `process.argv` para recibir argumentos desde la terminal.
- Manipulación de arrays mediante `slice()`.
- Estructuras condicionales (`if / else`).
- Estructura de control `switch`.
- Funciones asíncronas con `async / await`.
- Manejo de errores mediante `try / catch`.
- Consumo de APIs REST.
- Métodos HTTP: GET, POST y DELETE.
- Uso de `fetch()` para realizar solicitudes.
- Conversión de respuestas HTTP a formato JSON mediante `response.json()`.
- Envío de datos en formato JSON utilizando `JSON.stringify()`.

## API utilizada

**FakeStore API**

Documentación oficial: https://fakestoreapi.com/

Esta API permite realizar pruebas de consumo de servicios REST mediante diferentes operaciones sobre productos.

## Autora

**Juana Romero**

Estudiante de Analista de Sistemas.

Proyecto desarrollado como práctica de Node.js y consumo de APIs REST.
