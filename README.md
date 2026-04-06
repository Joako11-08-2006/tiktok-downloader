---

## 🚀 Tecnologías utilizadas

- Python 3.11
- Flask
- yt-dlp
- Docker

---

## 🧠 Descripción del proyecto

Esta aplicación permite al usuario ingresar un enlace de TikTok y descargar el video directamente desde el navegador.

El sistema utiliza la librería `yt-dlp` para procesar y descargar el contenido multimedia.

---

## ⚙️ Estructura del proyecto


tiktok-downloader/
│
├── app.py
├── requirements.txt
├── Dockerfile
├── Dockerfile.optimizado
├── Dockerfile.multistage
│
├── templates/
│ └── index.html
│
├── static/
│ └── style.css
│
└── videos/


---

## ▶️ Ejecución local

1. Instalar dependencias:


pip install -r requirements.txt


2. Ejecutar la aplicación:


python app.py


3. Abrir en navegador:


http://localhost:5000


---

## 🐳 Ejecución con Docker

### 🔹 Construir imagen


docker build -t tiktok:v1 .


### 🔹 Ejecutar contenedor


docker run -p 5000:5000 tiktok:v1


---

## ⚡ Versiones de Docker

Se implementaron tres versiones:

- **v1:** Dockerfile básico
- **v2:** Dockerfile optimizado (Alpine)
- **v3:** Dockerfile multi-stage (más eficiente)

---

## 🌐 Consideraciones

Debido a restricciones de virtualización en el entorno local, se utilizó GitHub Codespaces para la ejecución de Docker.

---

## 📊 Resultados

La aplicación funciona correctamente permitiendo:

- Ingresar una URL de TikTok  
- Descargar videos  
- Ejecutarse en contenedores Docker  

---

## 👨‍💻 Autor

- Joaquín Casas  
- Tecsup - Desarrollo de Software

---