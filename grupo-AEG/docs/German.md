# MARKDOWN DE EXPLICACIÓN DE GERMÄN
# 🚀 Guía Paso a Paso: Implementación de Sitios Web Estáticos con HUGO y MKDocs 🌐

¡Bienvenidos a esta guía completa! Aquí aprenderás cómo implementar tres tipos de sitios web estáticos utilizando HUGO y MKDocs. Cada sitio tendrá un propósito único y será desplegado en plataformas populares como GitHub Pages, Netlify y Cloudflare. ¡Manos a la obra! 💪


# Introducción

En la era de la transformación digital, los sitios web estáticos han resurgido como una solución eficiente y poderosa para crear contenido accesible, seguro y fácil de mantener. Herramientas modernas como **HUGO** y **MKDocs** nos permiten desarrollar sitios web dinámicos en apariencia, pero estáticos en su funcionamiento, ideales para blogs, portfolios o documentación técnica.

Este proyecto consta de tres tareas interconectadas que exploran la implementación y despliegue de sitios web utilizando tecnologías avanzadas y temas visualmente atractivos como **Ananke**, **PaperMod** y **Material**. Cada sitio web está diseñado para cumplir con propósitos específicos, desde blogs creativos hasta documentaciones profesionales, y se despliega en plataformas robustas como **GitHub Pages**, **Netlify** y **Cloudflare**.

En esta guía, aprenderás paso a paso cómo configurar tu entorno, desarrollar los sitios y desplegarlos en línea.
---

## 📝 **Tarea 1: Blog Sencillo con HUGO y Papermod**
Un blog estático con el tema **Papermdo**, desplegado en **GitHub Pages**.

---
### 🔧 **Paso 1: Configura tu entorno**
1. Instala [Hugo](https://gohugo.io/getting-started/installing/) en tu sistema.
2. Verifica la instalación con:
   ```bash
   hugo version

---
### 📂 Paso 2: Crea un nuevo proyecto
Crea un nuevo sitio llamado :actividad22_2_AEG
   ```bash
   hugo new site blog-actividad22_2_AEG
   ```
Navega al directorio:
   ```bash
   cd actividad22_2_AEG
   ```
---

### 🎨 Paso 3: Añade el tema Papermod
---

Descarga el tema:
   ```bash
   git init
   ```
   ```bash
   git submodule add https://adityatelange.github.io/hugo-PaperMod/posts/papermod/papermod-installation/
   ```
Configura el tema en config.toml:
toml
theme = "Papermod"

---
### ✍️ Paso 4: Crea tu contenido
Genera tu primer post:
  
   hugo new posts/primer-post.md

Edita el contenido en la carpeta content/posts/primer-post.md.

---
### 🔍 Paso 5: Prueba el sitio
Inicia un servidor local:

   hugo server


---
### ☁️ Paso 6: Despliega el sitio
- GitHub Pages:
Crea un repositorio en GitHub.
- Añade los archivos y haz un push:
   ```bash
   git add .
   git commit -m "subo el sitio"
   git branch -M main
   git remote add origin https://github.com/tu_usuario/blog-hugo-papermod.git
   git push -u origin main

Configura GitHub Pages desde la rama main.

Netlify:

- Crea una cuenta en Netlify.
- Conecta el repositorio y selecciona el directorio public/ como carpeta de publicación.

---

### 🌟 Tarea 2: Sitio Variado con HUGO y PaperMod
Un sitio estático con temática variada, usando el tema PaperMod, desplegado en GitHub Pages y Cloudflare.

---

### 🔧 Paso 1: Configura tu entorno
(Similar al Paso 1 de la Tarea 1).

### 📂 Paso 2: Crea un nuevo proyecto
Crea un sitio llamado sitio-variante:
bash
Copiar código
hugo new site sitio-variante
### 🎨 Paso 3: Añade el tema PaperMod
Descarga el tema:
bash
Copiar código
git submodule add https://github.com/adityatelange/hugo-PaperMod themes/PaperMod
Configura el tema en config.toml:
toml
Copiar código
theme = "PaperMod"
