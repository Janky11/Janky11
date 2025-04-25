<p align="center">
  <img src="https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/items/poke-ball.png" width="300" />
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
- 🗓️ **Fecha de Publicación:** 20/04/2025  

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
4. Modifica esta línea: app_location: "./sistemas-distribuidos"
5. app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"


## 🚦 Paso 3: Verifica la Acción de Despliegue

Haz clic en la pestaña **Actions** en la parte superior del repositorio.  
Busca el flujo de trabajo que se ejecutó automáticamente.  
Verifica que termine con estado **"completed"** ✅

---

## 🌐 Paso 4: Accede a tu Web App en Azure

Abre [portal.azure.com](https://portal.azure.com) e inicia sesión con tu cuenta institucional o de estudiante.  
Dirígete al servicio **Static Web Apps** y selecciona el nombre de tu app.

Haz clic en **Ir al recurso**, y luego verás un enlace URL con tu Pokédex funcionando online. ¡Dale clic y comprueba tu despliegue! 🔎

---

## 🧩 Paso 5: Configura Seguridad y Navegación
Desde tu repositorio: https://github.com/Janky11/Janky11  
Navega a: `sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/`

Haz clic en **Add file > Create new file**  
Nómbralo como: `staticwebapp.config.json`  
Y pega este contenido:

Desde tu repositorio: https://github.com/Janky11/Janky11  
Navega a: `sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/`

Haz clic en **Add file > Create new file**  
Nómbralo como: `staticwebapp.config.json`  
Y pega este contenido:
```json
{
  "globalHeaders": {
    "Content-Security-Policy": "default-src 'self'; img-src 'self' https://raw.githubusercontent.com https://pokeapi.co https://assets.pokemon.com; script-src 'self' 'unsafe-inline'; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src 'self' https://fonts.gstatic.com; connect-src 'self' https://beta.pokeapi.co",
    "X-Frame-Options": "DENY",
    "Permissions-Policy": "geolocation=(), microphone=(), camera=()"
  },
  "navigationFallback": {
    "rewrite": "/index.html",
    "exclude": ["/images/", "/css/", "/js/*", "/favicon.ico"]

## 🎉 ¡Listo! Tu Pokédex Está en la Nube

Tu Pokédex ya está activa en la web, lista para explorar, lucir increíble y capturar la atención de todos. 🧠  
¡Felicitaciones por completar el despliegue con estilo y seguridad!

---

## 🌟 Creador del Proyecto 🙌

🧙‍♂️ **Jean Carlos Orozco Imotila**  
_"Estudiante Apasionado de Ingeniería de Sistemas"_  

🔗 [GitHub](https://github.com/Janky11/Janky11) | 

🏆 **Habilidades Especiales:**
- 💻 **Desarrollo de Software**: Full Stack Developer (front-end + back-end).
- 🔐 **Ciberseguridad**: Protección de datos y redes.
- 🖥️ **Mantenimiento de Computadores**: Diagnóstico y reparación de equipos.
- 🎨 **Herramientas Digitales**: Excel, Photoshop.


📅 **Fecha de Creación del Proyecto**: 20/04/2025
}

