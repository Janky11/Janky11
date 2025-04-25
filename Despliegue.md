# 🧩 ¡Despliega tu Pokédex en Azure con Estilo! ⚡  
**🔗 Link de la web en la nube:** [https://witty-island-0d4269f10.6.azurestaticapps.net/](https://witty-island-0d4269f10.6.azurestaticapps.net/)  
✍️ **Autor:** Jean Carlos Orozco Imotila  
📂 **Repositorio:** [https://github.com/Janky11/Janky11](https://github.com/Janky11/Janky11)  
📚 **Asignatura:** Sistemas Distribuidos  
🎓 **Semestre:** 9no semestre - Ingeniería de Sistemas  
📅 **Fecha:** 13/04/2025  

---

## ☁️ ¡Prepárate para llevar tu Pokédex a la nube de una manera súper sencilla y visual!  

---

### 1️⃣ 🍽️ ¡A Bifurcar el Código! (Forking Time!)  

Ve directo al corazón del código Pokédex:  
🔗 [https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab](https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab)

- Haz clic en el botón **Fork** (esquina superior derecha) 👆  
- Nombra tu copia como prefieras, por ejemplo: `Janky11`  
- Presiona **Create fork** 🎉  

---

### 2️⃣ 📁 ¡Navegando a la Ubicación Correcta! (App Location Adventure!)  

🏡 Dirígete a tu repo forkeado:  
[https://github.com/Janky11/Janky11](https://github.com/Janky11/Janky11)

- Entra a la carpeta: `.github/workflows/`  
- Abre el archivo: `azure-static-web-apps-<algo>.yml`  
- Da clic en el ícono del lápiz ✏️ para editar  
- Busca esta línea (aprox. línea 31):

```yml
app_location: "./sistemas-distribuidos"
###🔁 ¡Cámbiala por esta ruta mágica! ✨
app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"

###3️⃣ 🎬 ¡Luces, Cámara, Actions! (Checking the Magic!)
Haz clic en la pestaña Actions en tu repositorio

Verifica que el workflow se esté ejecutando con éxito 🚦

Espera hasta que esté completado 🟢

###4️⃣ 🌐 ¡Despegue a la Nube de Azure! (Azure Deployment!)
Ve al portal de Azure: https://portal.azure.com

Ingresa a App Services

Haz clic sobre tu Static Web App

Da clic en Ir al recurso

🌍 ¡Abre el enlace en la sección URL y admira tu Pokédex en acción!

###5️⃣ 🛡️ ¡Escudos de Seguridad y Rutas Inteligentes! (Security & Navigation!)
Regresa a tu repo: https://github.com/Janky11/Janky11

Navega a:
sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/

Crea un nuevo archivo llamado: staticwebapp.config.json

Pega el siguiente contenido 🔒:
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
Guarda con Commit changes ✅

Vuelve a Actions y espera a que finalice el despliegue 🎉

###6️⃣ 🖼️ ¡Dando Vida a los Pokémon con Imágenes! (Loading Pokemon Images!) 🎨
Ve a la ruta:
sistemas-distribuidos/poke-dex-lab/source/pokedex-angular/src/environments/

Abre y edita el archivo environment.prod.ts ✏️

Reemplaza esta línea:
imagesPath: 'pokedex-angular/assets/images',
###🔁 Por esta:
imagesPath: '/assets/images',
Guarda los cambios con Commit changes ✅

Verifica el workflow en Actions. ¡Tus Pokémon ya deberían tener cara! 😄

###🎉 ¡Felicidades!
Has desplegado tu Pokédex en Azure Static Web Apps como todo un experto en la nube.
¡Atraparlos a todos ahora es digitalmente épico! 💾🔥

###✨ Creador del Proyecto
###🧑‍💻 Jean Carlos Orozco Imotila
###Estudiante apasionado de Ingeniería de Sistemas - 9no semestre
