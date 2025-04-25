# 🚀 ¡Despliega tu Pokedex en Azure con Estilo! 🌟  
**Link de la web en la nube:** https://delightful-field-02ef8bb10.6.azurestaticapps.net/  
✍️ **Autor:** Jean Carlos Orozco Imotila  
📂 **Repositorio:** https://github.com/Albertohincapie11/albertacho  
📚 **Asignatura:** Sistemas Distribuidos  
🎓 **Semestre:** 9no semestre - Ingeniería de Sistemas  
📅 **Fecha:** 13/04/2025  

---

## ¡Prepárate para llevar tu Pokedex a la nube de una manera súper sencilla y visual! ☁️

---

### 1. 🎓 ¡Regístrate como Estudiante en Azure! (¡Gratis!) 📘  

1. Ingresa a [https://azure.microsoft.com/free/students/](https://azure.microsoft.com/free/students/)  
2. Haz clic en **"Iniciar gratis"**.  
3. Inicia sesión con tu cuenta institucional (.edu o de estudiante).  
4. Completa el formulario con tus datos personales y confirma tu cuenta de estudiante.  
5. ¡Listo! Ahora tienes acceso gratuito a servicios de Azure con $100 USD en crédito para estudiantes. 🎉  

---

### 2. 🍴 ¡A Bifurcar el Código! (Forking Time!) 🛠️  

🔗 Código base: [Pokedex Lab](https://github.com/rcuello/ac4dem1a/tree/master/sistemas-distribuidos/poke-dex-lab)  
- Haz clic en **Fork** en la esquina superior derecha.  
- Nombra tu copia como prefieras, por ejemplo: `albertacho`.  
- Da clic en **Create fork**.

---

### 3. 🗺️ ¡Navegando a la Ubicación Correcta! (App Location Adventure!) 🧭  

1. Visita tu repositorio forkeado: `https://github.com/tu-usuario/tu-repo`  
2. Dirígete a: `.github/workflows/`  
3. Abre y edita el archivo `azure-static-web-apps-*.yml`  
4. Encuentra esta línea (aprox. línea 31):

```yml
app_location: "./sistemas-distribuidos"
Remplaza
app_location: "./sistemas-distribuidos/poke-dex-lab/source/pokedex-angular"

