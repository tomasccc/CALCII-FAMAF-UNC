# **Guía de Contribución**

Hay dos formas de colaborar: desde el navegador, o descargando el código fuente y trabajando localmente, para luego enviar tus cambios a través de un Pull Request.

---

### **Opción 1: Editor Web**

El repositorio tiene un editor integrado directamente en el sitio (Decap CMS) para que puedas escribir y previsualizar tus apuntes en tiempo real, sin instalar nada.

### 1. Iniciar Sesión
1. Entrá al panel de administración haciendo click en el botón de edición (✏️ si estás en tu computadora, y al final de la nota si estás en celular). (o podés agregar `/admin` al final de la URL del sitio).
2. Hacé clic en **"Login with GitHub"**. 
3. Te va a pedir autorización para conectar tu cuenta. Dale a aceptar. *(El manejo de tus datos en su totalidad pasa por Github, por lo que no se almacena absolutamente nada referido a tu identidad. El sitio simplemente consulta quiénes contribuyeron al apunte cuando lo vés en la página.).*

### 2. Crear tu apunte y organizar las carpetas
Una vez adentro, vas a ver las colecciones a la izquierda (Oficial y Comunidad con las subcarpetas). Elegí la que corresponda y hacé clic en **"New"** (Nuevo).

!!! tip "Organización de Carpetas 📁"
    En la parte superior del editor vas a ver un campo llamado **Destino del apunte**. Acá tenés dos opciones:

    * **Para un apunte suelto:** Dejá escrita la palabra `general`.
    * **Para crear una carpeta nueva:** Borrá "general" y escribí el nombre de tu nueva carpeta **SIN ESPACIOS** (usá guiones). Por ejemplo: `unidad-4-integrales`.

### 3. Fórmulas Matemáticas
El editor tiene una pantalla dividida: a la izquierda escribís y a la derecha se visualiza cómo va quedando tu nota. 

!!! warning "Saltos de línea y previsualización"
    * Para que las ecuaciones grandes (las que van entre `$$`) se previsualicen bien y no rompan el formato, **siempre debés dejar un renglón en blanco antes y después** de la fórmula.

    * Para las fórmulas pequeñas (entre `$`) no es necesario dejar un renglón en blanco, pero sí es recomendable dejar uno o dos espacios antes y después de la fórmula para que se visualice correctamente.

### 4. Guardar y Publicar
Antes de guardar, acordate de ir al menú desplegable de "Autoría y Responsabilidad" y seleccionar **Acepto**. Esto confirma que el apunte es tuyo y se publicará gratis para todos. Finalmente, dale al botón verde de **Publish** (Publicar). El sistema se encarga de enviarnos tu apunte.

Al subir material a través de Pull Requests o del editor web (Decap CMS), declarás que sos el autor de dicho contenido o tenés permiso para compartirlo. Al hacerlo, aceptás que tu aporte sea publicado bajo la licencia **CC BY-NC-SA 4.0**. El administrador se reserva el derecho de remover material que infrinja derechos de autor de terceros.

---

### **Opción 2: (Fork & Pull Request)**

Si preferís contribuir de manera más avanzada, preferís usar un editor de texto o IDE, o querés tener una copia local del repositorio, podés descargar el código fuente, hacer tus cambios y luego enviar un Pull Request para que tus aportes sean revisados e integrados al proyecto. Esto es lo que hace el sistema de forma automática cuando usás el editor web, pero esta opción te da más control sobre el proceso.

### 1. Forkear el repositorio
1. Entrá a nuestro repositorio oficial en GitHub.
2. Arriba a la derecha, hacé clic en el botón **Fork**. Esto creará una copia exacta del proyecto en tu propia cuenta de GitHub.

### 2. Clonar y crear una rama
Abrí tu terminal y bajate tu copia (cambiá "TuUsuario" por tu nombre de GitHub):
```bash
git clone [https://github.com/TuUsuario/CALCII-FAMAF-UNC.git](https://github.com/TuUsuario/CALCII-FAMAF-UNC.git)
cd CALCII-FAMAF-UNC