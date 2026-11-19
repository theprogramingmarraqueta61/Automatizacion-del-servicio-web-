# Integración con GitHub

## Código fuente publicado

El código fuente del sitio web de la práctica se encuentra en la carpeta `sitio_web/`, acompañada por la configuración de Nginx en `docker/`.

## Importancia del control de versiones

GitHub permite registrar los cambios realizados sobre el código, mantener versiones anteriores y facilitar el trabajo colaborativo.

## Por qué no sustituye un respaldo Docker

El repositorio Git conserva el código y los archivos versionados, pero no equivale automáticamente a una copia de seguridad de una imagen Docker o del estado completo de un entorno de ejecución. Por ello, el respaldo Docker y el control de versiones deben considerarse mecanismos complementarios.

- GitHub: control de versiones y recuperación del código fuente.
- Respaldo Docker: recuperación de imágenes/artefactos del entorno Docker que se hayan respaldado.

Esta separación permite recuperar el código y, por otra vía, recuperar el entorno Docker cuando sea necesario.
