# API-de-Usuarios-con-FastAPI-y-MongoDB
Este proyecto implementa una API REST utilizando FastAPI para la gestión de usuarios, con operaciones CRUD (Crear, Leer, Actualizar y Eliminar) y persistencia de datos en una base de datos MongoDB.

## Descripción

La API permite gestionar usuarios, almacenando su información en una base de datos MongoDB. Se utilizan Pydantic para la validación de datos y APIRouter para organizar las rutas de la API de manera modular.

## Tecnologías Utilizadas

*   **FastAPI:** Framework web de alto rendimiento para Python.
*   **Pymongo:** Driver de Python para MongoDB.
*   **Pydantic:** Librería para la validación y serialización de datos.
*   **Uvicorn:** Servidor ASGI para ejecutar la aplicación FastAPI.

## Configuración de MongoDB

1.  Asegúrate de tener MongoDB instalado y en ejecución.
2.  Puedes configurar la conexión a MongoDB de dos maneras:
    *   **Variables de entorno:** Define la variable de entorno `MONGODB_URL` con la URL de conexión a tu base de datos MongoDB. Por ejemplo:

        ```
        MONGODB_URL=mongodb://usuario:contraseña@host:puerto/nombre_de_la_base_de_datos
        ```

## Ejecución

```bash
uvicorn main:app --reload
