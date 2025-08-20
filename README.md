## Descripción

Este repositorio contiene una aplicación web de machine learning que utiliza el framework Flask y un modelo entrenado con PyCaret. La aplicación está empaquetada en un contenedor Docker para facilitar su despliegue.

## Estructura del Proyecto

- `Dockerfile`: Define los pasos para construir la imagen del contenedor.
- `app.py`: El código de la aplicación Flask que carga el modelo y expone un endpoint para las predicciones.
- `requirements.txt`: Lista de dependencias de Python.
- `model.pkl`: El modelo de machine learning entrenado y serializado.

## Cómo ejecutar el proyecto

1.  **Construye la imagen de Docker:**
    ```bash
    docker build -t nombre-de-tu-imagen .
    ```
2.  **Ejecuta el contenedor:**
    ```bash
    docker run -p 5000:5000 nombre-de-tu-imagen
    ```
