# 📄 Informe Técnico: Docker

## 🎥 Video #1 – Introducción a Docker

El primer video presenta una explicación general sobre Docker y su función dentro del desarrollo de software. Se describe a Docker como una plataforma que permite crear, ejecutar y administrar aplicaciones dentro de contenedores, facilitando la portabilidad y el control del entorno de ejecución.

### Conceptos destacados

- Un **contenedor** es un entorno ligero que incluye el código de la aplicación, librerías y dependencias necesarias para su funcionamiento.
- Docker permite que una aplicación se ejecute de manera consistente sin importar el sistema operativo.
- Las **imágenes Docker** son estructuras inmutables que sirven como base para crear contenedores.
- El **Dockerfile** es el archivo donde se definen las instrucciones para construir una imagen personalizada.
- **Docker Hub** funciona como un repositorio público para almacenar y compartir imágenes Docker.

---

## 🎥 Video #2 – Uso Práctico de Docker

El segundo video se enfoca en el uso práctico de Docker, mostrando cómo instalarlo y cómo trabajar con contenedores desde la línea de comandos.

### Temas abordados

- Instalación básica de Docker en el sistema operativo.
- Comandos fundamentales:
  - `docker pull` para descargar imágenes.
  - `docker run` para ejecutar contenedores.
  - `docker ps` para listar contenedores activos.
  - `docker stop` y `docker rm` para detener y eliminar contenedores.
- Creación de aplicaciones propias mediante Dockerfile.
- Uso del archivo `docker-compose.yml` para administrar múltiples servicios, como una aplicación y su base de datos.

---

## 🤔 Reflexiones

### Ventajas
Docker facilita la configuración de entornos de desarrollo y mejora la portabilidad de las aplicaciones. Es especialmente útil en trabajos colaborativos, ya que todos los integrantes del equipo pueden trabajar bajo las mismas condiciones.

### Desafíos
El uso de Docker requiere comprender conceptos como imágenes, capas y redes. Además, una mala construcción de imágenes puede generar conflictos de versiones o un uso innecesario de espacio.

### Uso práctico
Docker es ideal para proyectos donde se utilizan varios servicios, como APIs con bases de datos y frontend, o cuando es necesario asegurar que las pruebas se ejecuten de forma idéntica en distintos entornos.

---

## 🧪 Ejemplo Práctico: Hola Mundo en Docker

En este ejemplo se crea una aplicación sencilla utilizando Python y Flask, la cual se ejecuta dentro de un contenedor Docker.

---

### 📁 Archivos del proyecto

Dentro de Visual Studio Code se crean los siguientes archivos:

- `Dockerfile`
- `app.py`
- 
<img width="921" height="701" alt="image" src="https://github.com/user-attachments/assets/4bfa9ea6-ec86-46f0-bb03-db68bb9bcc22" />
---

### 📄 Archivo Dockerfile

<img width="921" height="508" alt="image" src="https://github.com/user-attachments/assets/da02f72d-b510-4763-8380-fa3c3d208ac9" />

▶️ Construcción de la imagen

Para crear la imagen Docker se ejecuta el siguiente comando en la terminal:

docker build -t miappdocker .

<img width="921" height="547" alt="image" src="https://github.com/user-attachments/assets/856ecc27-1ed1-4fe7-9ad3-9c9be9ebc01c" />

▶️ Ejecución del contenedor

Luego se ejecuta el contenedor con el comando:

docker run -p 5000:5000 miappdocker

 <img width="921" height="157" alt="image" src="https://github.com/user-attachments/assets/16bdff7f-5458-4709-b83c-c08ef153f00a" />

Al abrir el navegador en la siguiente dirección:

http://localhost:5000

Se mostrará el mensaje:

<img width="673" height="331" alt="image" src="https://github.com/user-attachments/assets/b46f84d1-95bc-447a-9f99-5e3abfbcc90c" />

