# Automatización del servicio web

Proyecto académico de Sistemas Operativos orientado a documentar la configuración y automatización del servicio web Nginx en Alpine Linux, correspondiente al ticket INC-05.

## Integrantes

- Gerardo Gutierrez Rosales
- Leonardo Garcia Mendoza
- Gabriel Zerpa Diaz
- Santiago Beltran Menini

## Contenido del proyecto

Este repositorio reúne la documentación y las evidencias del trabajo de automatización del servicio web, incluyendo el diagnóstico del inicio de Nginx, su configuración para arrancar automáticamente, la programación del horario laboral mediante cron y las pruebas de funcionamiento.

También incorpora el código fuente del sitio web utilizado en Docker, para cumplir con la integración del código fuente en GitHub.

## Código fuente del sitio web

El sitio web está organizado en:

- `sitio_web/index.html`: página principal personalizada.
- `sitio_web/50x.html`: página de error utilizada por Nginx.
- `docker/default.conf`: configuración de Nginx para servir el sitio desde `/usr/share/nginx/html`.

El sitio está preparado para ser servido por Nginx y el contenido HTML corresponde al sitio utilizado en la práctica del Hito 4.

## Integración con GitHub

Publicar el código fuente en GitHub permite mantener un historial de cambios, identificar versiones anteriores, comparar modificaciones y trabajar de forma colaborativa. GitHub funciona como repositorio de control de versiones del código y de la documentación del proyecto.

### ¿Por qué GitHub no sustituye un respaldo Docker?

El control de versiones y un respaldo Docker cumplen funciones diferentes:

- **Git/GitHub** conserva principalmente archivos del proyecto y su historial de modificaciones.
- **Un respaldo Docker** puede conservar una imagen o los elementos necesarios para recuperar un entorno de ejecución concreto, incluyendo el estado de la aplicación empaquetado en una imagen.
- Tener el código en GitHub no garantiza por sí solo que se conserve una imagen Docker específica, sus capas, el estado de un contenedor o un entorno que ya no pueda reconstruirse exactamente.
- Por eso, GitHub debe utilizarse como control de versiones del código fuente, mientras que los respaldos Docker deben mantenerse como mecanismo complementario para recuperación del entorno.

En conclusión, GitHub permite recuperar y gestionar el código fuente, pero no reemplaza una estrategia de respaldo de las imágenes, configuraciones y demás elementos necesarios para recuperar el entorno Docker.

## Informe

Informe principal: `Informe_INC-05_Automatizacion_Servidor_Web.docx`.

## Entorno

- Servicio web: Nginx
- Sistema operativo: Alpine Linux
- Asignatura: Sistemas Operativos · Paralelo 2
- Institución: Universidad Privada Franz Tamayo (Unifranz)
