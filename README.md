# Introducción a Docker 🐳

Docker es una plataforma que permite desarrollar, enviar y ejecutar aplicaciones dentro de contenedores. Los contenedores son entornos ligeros, portables y autosuficientes que incluyen todo lo necesario para ejecutar una aplicación: código, dependencias, librerías y configuraciones.

## ¿Por qué usar Docker?

- 🔁 Portabilidad entre entornos (desarrollo, testing, producción)
- 🧩 Aislamiento de servicios y aplicaciones
- 🚀 Despliegues rápidos y consistentes
- 💡 Facilita la integración continua y la entrega continua (CI/CD)

## Instalación

Puedes instalar Docker desde su sitio oficial:  
👉 [https://docs.docker.com/get-docker/](https://docs.docker.com/get-docker/)

Una vez instalado, verifica la instalación con:

## Comandos Esenciales

### 🔍 Información básica

- `docker --version`  
  Muestra la versión instalada de Docker.

- `docker info`  
  Muestra detalles del sistema Docker (configuración, contenedores, imágenes, etc).

### 🖼️ Imágenes

- `docker pull <imagen>`  
  Descarga una imagen desde Docker Hub.

- `docker images`  
  Lista todas las imágenes locales.

- `docker rmi <imagen>`  
  Elimina una imagen.

### 📦 Contenedores

- `docker run <imagen>`  
  Ejecuta un contenedor basado en una imagen.

- `docker run -it <imagen> /bin/bash`  
  Ejecuta un contenedor con una terminal interactiva.

- `docker ps`  
  Muestra los contenedores en ejecución.

- `docker ps -a`  
  Muestra todos los contenedores (en ejecución y detenidos).

- `docker stop <id_contenedor>`  
  Detiene un contenedor en ejecución.

- `docker start <id_contenedor>`  
  Inicia un contenedor detenido.

- `docker restart <id_contenedor>`  
  Reinicia un contenedor.

- `docker rm <id_contenedor>`  
  Elimina un contenedor detenido.

- `docker exec -it <id_contenedor> bash`  
  Abre una terminal dentro de un contenedor en ejecución.

- `docker logs <id_contenedor>`  
  Muestra los registros del contenedor.

### 🛠️ Imágenes personalizadas
 
- `docker build -t <nombre_imagen> .`  
  Construye una imagen desde un `Dockerfile` en el directorio actual.

