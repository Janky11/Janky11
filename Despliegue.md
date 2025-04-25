<!-- Encabezado visual -->
<p align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNzh2M2V0N2s5aWJmbDB0OTJpNXY3MWdzZG1jdGk5dThudm5sMGMwNCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/3oEjI6SIIHBdRxXI40/giphy.gif" width="280px">
</p>

<h1 align="center">🎮 PokeDeploy: Tu Pokédex en la Nube con Azure 🎮</h1>

<p align="center">
  Una guía rápida y divertida para publicar tu app Pokémon usando servicios de Microsoft Azure 🌥️
</p>

---

<p align="center">
  <img src="https://img.shields.io/badge/AZURE--STATIC--WEB--APP-DESPLEGADO-blueviolet?style=for-the-badge&logo=azuredevops">
  <img src="https://img.shields.io/badge/SEMESTRE-9°--SISTEMAS-orange?style=for-the-badge">
  <img src="https://img.shields.io/badge/STATUS-%F0%9F%92%AA%20ACTIVO-green?style=for-the-badge">
</p>

---

### 📍 Información General

- 🌐 **Web App Activa:** [https://witty-island-0d4269f10.6.azurestaticapps.net](https://witty-island-0d4269f10.6.azurestaticapps.net)
- 📘 **Repositorio de Trabajo:** [https://github.com/Janky11/Janky11](https://github.com/Janky11/Janky11)
- 🧠 **Materia:** Sistemas Distribuidos
- 🧑‍💻 **Autor:** Jean Carlos Orozco Imotila  
- 🎓 **Semestre:** Noveno (Ingeniería de Sistemas)  
- 🗓️ **Fecha de Publicación:** 13/04/2025  

---

## 🧭 Guía de Despliegue Paso a Paso

### 🔁 Paso 1: Clona el Proyecto Base

Accede al código fuente original:  
📎 [Repositorio de Referencia](https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab)

- Haz clic en el botón **Fork**
- Crea tu propia versión del repo
- Asígnale un nombre representativo (ej: `Janky11`)

---

### ⚙️ Paso 2: Ajustes del Proyecto

1. Dirígete a tu fork en: [https://github.com/Janky11/Janky11](https://github.com/Janky11/Janky11)
2. Accede a: `.github/workflows/`
3. Localiza el archivo `.yml` de despliegue (puede tener un nombre similar a `azure-static-web-apps-*.yml`)
4. Modifica esta línea:

```yml
app_location: "./sistemas-distribuidos"
🔁 Sustitúyela por:

yml
Copiar
Editar
app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"
✔️ Guarda tus cambios con un commit

### ⚡ Paso 3: Ejecuta y Revisa el Despliegue
En la pestaña Actions del repositorio, monitorea que el flujo de trabajo se ejecute correctamente.

Espera hasta que aparezca como completado.

🔍 Paso 4: Explora tu Pokédex en Azure
Accede al portal de Azure: https://portal.azure.com

Selecciona tu Static Web App

Entra al recurso para obtener el enlace público de tu aplicación

🔐 Paso 5: Agrega Configuración de Seguridad
Desde tu repositorio, ve a: sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/

Crea un nuevo archivo: staticwebapp.config.json

Inserta este contenido:

json
Copiar
Editar
{
  "globalHeaders": {
    "Content-Security-Policy": "default-src 'self'; img-src 'self' https://raw.githubusercontent.com https://pokeapi.co https://assets.pokemon.com; script-src 'self' 'unsafe-inline'; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src 'self' https://fonts.gstatic.com; connect-src 'self' https://beta.pokeapi.co",
    "X-Frame-Options": "DENY",
    "Permissions-Policy": "geolocation=(), microphone=(), camera=()"
  },
  "navigationFallback": {
    "rewrite": "/index.html",
    "exclude": ["/images/", "/css/", "/js/*", "/favicon.ico"]
  }
}
🔁 Espera que se ejecute de nuevo el flujo en Actions

🖼️ Paso 6: Visualiza tus Pokémon con Estilo
Dirígete a:
sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/src/environments/

Edita el archivo environment.prod.ts

Reemplaza:

ts
Copiar
Editar
imagesPath: 'pokedex-angular/assets/images',
🔁 Por:

ts
Copiar
Editar
imagesPath: '/assets/images',
✅ Realiza el commit y espera que el proceso se ejecute exitosamente.

🧑‍🎓 Sobre el Autor
Jean Carlos Orozco Imotila
Noveno semestre de Ingeniería de Sistemas
