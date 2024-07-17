# Aplicación de Recetas

![img-portada](img-portada2.png)

## 🚀 Sobre el proyecto <a name = "about"></a>

Este proyecto es una aplicación web de recetas desarrollada como parte del Trabajo Práctico Integrador para la materia Programación 3. La aplicación utiliza ReactJS para el frontend y una API RESTful para consumir y manipular datos.

El objetivo es demostrar los conocimientos adquiridos durante el curso, incluyendo autenticación, manejo de sesiones, y operaciones CRUD (Create, Read, Update, Delete).

## 📝 Índice
- [Sobre el proyecto](#about)
- [Instalación](#installation)
- [Estructura del proyecto](#project-structure)
- [Funcionalidades](#functionalities)
- [API](#api)
  - [Recipe Categories](#recipe-categories)
  - [Comments](#comments)
  - [Ingredients](#ingredients)
  - [Recipe Locations](#recipe-locations)
  - [Recipes](#recipes)
  - [Recipe Ingredients](#recipe-ingredients)
  - [Steps](#steps)
- [Tecnologías utilizadas](#technologies)
- [Autores](#authors)

## ⚙️ Instalación <a name = "installation"></a>

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/paunicole/app-musica.git
   ```

2. **Navega al directorio del proyecto:**
   ```bash
   cd app-musica
   ```

3. **Instala las dependencias:**
   ```bash
   npm install
   ```

4. **Ejecuta la aplicación en modo desarrollo:**
   ```bash
   npm start
   ```

## 🏛️ Estructura del proyecto <a name = "project-structure"></a>

```bash
raíz del proyecto
├───src/
│   ├───components/
│   ├───pages/
│   ├───services/
│   ├───App.js
│   ├───index.js
```

## ⚡ Funcionalidades <a name = "functionalities"></a>

### Login
Permite a los usuarios autenticarse en la aplicación utilizando JWT.

### Registro de Usuarios
Permite a los nuevos usuarios registrarse en la aplicación.

### Navegación
Incluye rutas para navegar entre diferentes secciones de la aplicación:

| URL        | Descripción                               |
|------------|-------------------------------------------|
| /          | Página de inicio con una lista de recetas |
| /login     | Página de inicio de sesión                |
| /profile   | Página de perfil de usuario               |

### CRUD de Recetas
Permite crear, leer, actualizar y eliminar recetas a través de formularios.

## 🗺 API <a name = "api"></a>

### Recipe Categories <a name = "recipe-categories"></a>

| URL                              | Método | Descripción                                         |
|----------------------------------|--------|-----------------------------------------------------|
| /reciperover/categories/         | GET    | Lista todas las categorías de recetas               |
| /reciperover/categories/         | POST   | Asigna una nueva categoría a una receta             |
| /reciperover/categories/{id}     | GET    | Detalles de una categoría de una receta             |
| /reciperover/categories/{id}     | PUT    | Actualiza una categoría de una receta               |
| /reciperover/categories/{id}     | PATCH  | Actualiza parcialmente una categoría de una receta  |
| /reciperover/categories/{id}     | DELETE | Elimina una categoría de una receta                 |

| URL                                   | Método | Descripción                                         |
|---------------------------------------|--------|-----------------------------------------------------|
| /reciperover/recipes/categories/      | GET    | Lista todas las categorías de recetas               |
| /reciperover/recipes/categories/      | POST   | Asigna una nueva categoría a una receta             |
| /reciperover/recipes/categories/{id}  | GET    | Detalles de una categoría de una receta             |
| /reciperover/recipes/categories/{id}  | PUT    | Actualiza una categoría de una receta               |
| /reciperover/recipes/categories/{id}  | PATCH  | Actualiza parcialmente una categoría de una receta  |
| /reciperover/recipes/categories/{id}  | DELETE | Elimina una categoría de una receta                 |

### Comments

| URL                         | Método | Descripción                                        |
|-----------------------------|--------|----------------------------------------------------|
| /reciperover/comments/      | GET    | Lista todos los comentarios de recetas             |
| /reciperover/comments/      | POST   | Crea un nuevo comentario a una receta              |
| /reciperover/comments/{id}  | GET    | Detalles de un comentario                          |
| /reciperover/comments/{id}  | PUT    | Actualiza un comentario de una receta              |
| /reciperover/comments/{id}  | PATCH  | Actualiza parcialmente un comentario de una receta |
| /reciperover/comments/{id}  | DELETE | Elimina un comentario de una receta                |

### Ingredients

| URL                             | Método | Descripción                           |
|---------------------------------|--------|---------------------------------------|
| /reciperover/ingredients/       | GET    | Lista todos los ingredientes          |
| /reciperover/ingredients/       | POST   | Crea un nueva ingrediente             |
| /reciperover/ingredients/{id}   | GET    | Detalles de un ingrediente            |
| /reciperover/ingredients/{id}   | PUT    | Actualiza un ingrediente              |
| /reciperover/ingredients/{id}   | PATCH  | Actualiza parcialmente un ingrediente |
| /reciperover/ingredients/{id}   | DELETE | Elimina un ingrediente                |

### Recipe Locations

| URL                             | Método | Descripción                                                                    |
|---------------------------------|--------|--------------------------------------------------------------------------------|
| /reciperover/locations/         | GET    | Lista todas las ubicaciones donde se puede encontrar una preparación de receta |
| /reciperover/locations/         | POST   | Asigna una nueva ubicación donde se puede encontrar una preparación de receta  |
| /reciperover/locations/{id}     | GET    | Detalles de una ubicación donde se puede encontrar una preparación de receta   |
| /reciperover/locations/{id}     | PUT    | Actualiza una ubicación de una receta                                          |
| /reciperover/locations/{id}     | PATCH  | Actualiza parcialmente una ubicación de una receta                             |
| /reciperover/locations/{id}     | DELETE | Elimina una ubicación de una receta                                            |

| URL                                  | Método | Descripción                                                                     |
|--------------------------------------|--------|---------------------------------------------------------------------------------|
| /reciperover/recipes/locations/      | GET    | Lista todas las ubicaciones donde se puede encontrar una preparación de receta  |
| /reciperover/recipes/locations/      | POST   | Asigna una nueva ubicación donde se puede encontrar una preparación de receta   |
| /reciperover/recipes/locations/{id}  | GET    | Detalles de una ubicación donde se puede encontrar una preparación de receta    |
| /reciperover/recipes/locations/{id}  | PUT    | Actualiza una ubicación de una receta                                           |
| /reciperover/recipes/locations/{id}  | PATCH  | Actualiza parcialmente una ubicación de una receta                              |
| /reciperover/recipes/locations/{id}  | DELETE | Elimina una ubicación de una receta                                             |

### Recipes

| URL                         | Método | Descripción                       |
|-----------------------------|--------|-----------------------------------|
| /reciperover/recipes/       | GET    | Lista todos las recetas           |
| /reciperover/recipes/       | POST   | Crea un nueva receta              |
| /reciperover/recipes/{id}   | GET    | Detalles de una receta            |
| /reciperover/recipes/{id}   | PUT    | Actualiza una receta              |
| /reciperover/recipes/{id}   | PATCH  | Actualiza parcialmente una receta |
| /reciperover/recipes/{id}   | DELETE | Elimina una receta                |

### Recipe Ingredients

| URL                                     | Método | Descripción                                         |
|-----------------------------------------|--------|-----------------------------------------------------|
| /reciperover/recipes/ingredients/       | GET    | Lista todos los ingredientes de recetas             |
| /reciperover/recipes/ingredients/       | POST   | Asigna un nuevo ingrediente a una receta            |
| /reciperover/recipes/ingredients/{id}   | GET    | Detalles de un ingrediente de una receta            |
| /reciperover/recipes/ingredients/{id}   | PUT    | Actualiza un ingrediente de un receta               |
| /reciperover/recipes/ingredients/{id}   | PATCH  | Actualiza parcialmente un ingrediente de una receta |
| /reciperover/recipes/ingredients/{id}   | DELETE | Elimina un ingrediente de una receta                |

### Steps

| URL                            | Método | Descripción                                    |
|--------------------------------|--------|------------------------------------------------|
| /reciperover/steps             | GET    | Lista todos los pasos de recetas disponibles   |
| /reciperover/steps             | POST   | Crea un nuevo paso para una receta             |
| /reciperover/steps/{id}        | GET    | Detalles de un paso de receta                  |
| /reciperover/steps/{id}        | PUT    | Actualiza un paso de un receta                 |
| /reciperover/steps/{id}        | PATCH  | Actualiza parcialmente un paso de una receta   |
| /reciperover/steps/{id}        | DELETE | Elimina un paso                                |

## ⛏️ Tecnologías utilizadas <a name = "technologies"></a>
- ReactJS
- API RESTful (con autenticación JWT)
- Git para control de versiones
- Vercel/Netlify para despliegue

## ✒️ Autoras <a name = "authors"></a>

| [<img src="https://avatars.githubusercontent.com/u/140465346?v=4" width=115><br><sub>Ivana Maidana</sub>](https://github.com/IvanaTwT) |  [<img src="https://avatars.githubusercontent.com/u/129181094?v=4" width=115><br><sub>Nicole Cardozo Gómez</sub>](https://github.com/paunicole) |
| :---: | :---: |
