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
🔁 ¡Cámbiala por esta ruta mágica! ✨
app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"


