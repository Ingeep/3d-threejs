# 🌐 Proyectos 3D con Three.js & WebGL

Colección de escenas interactivas en 3D desarrolladas con **Three.js** y **WebGL** para la asignatura de **Computación Gráfica II** (Universidad Central del Este - UCE).

---

## 🚀 Demo en Vivo

Puedes explorar e interactuar con los proyectos directamente en tu navegador sin instalar nada:

👉 **[Ver Proyecto en GitHub Pages](https://ingeep.github.io/3d-threejs/)**

---

## 📦 Escenas Incluidas

El proyecto cuenta con un menú principal (`index.html`) que permite navegar entre las siguientes escenas:

### 1. 🏠 Casa 3D (`Casa.html`)
* **Modelado arquitectónico completo:** Estructura modular de dos niveles con garaje, porche y caminos exteriores.
* **Mapeo de texturas:** Texturas mapeadas con repetición (ladrillo, césped, tejas, madera rústica, piedra, cristales y portón de garaje).
* **Tejados piramidales:** Alineados geométricamente con las paredes cuadradas mediante rotación en radianes (`Math.PI / 4`).
* **Iluminación realista:** Combinación de `AmbientLight` para relleno y `DirectionalLight` (luz solar) con sombras dinámicas suaves (`PCFSoftShadowMap`).
* **Materiales:** Uso de `MeshLambertMaterial` para superficies difusas y `MeshPhongMaterial` transparente para los cristales de la ventana.

### 2. 🦒 Jirafa 3D (`Jirafa.html`)
* **Modelado procedural:** Construcción anatómica detallada a partir de primitivas geométricas (`BoxGeometry`).
* **Detalles anatómicos:** Patas articuladas divididas en secciones, cuerpo escalonado, cuello alargado, orejas, antenas y manchas volumétricas posicionadas alrededor de la piel.
* **Escenario:** Suelo plano texturizado con césped y sistema de iluminación ambiental y direccional.

---

## 🎮 Controles de Navegación 3D

Ambas escenas utilizan `OrbitControls` para permitir una exploración libre:

| Acción | Control del Ratón |
| :--- | :--- |
| **Rotar la cámara** | Clic izquierdo + arrastrar |
| **Zoom (Acercar / Alejar)** | Rueda del ratón (Scroll) |
| **Desplazar vista (Pan)** | Clic derecho + arrastrar |
| **Volver al menú** | Botón flotante `← Volver al Menú` |

---

## 🛠️ Tecnologías Utilizadas

* **JavaScript (Vanilla)**
* **[Three.js](https://threejs.org/)** (v144)
* **WebGL API**
* **OrbitControls.js**
* **HTML5 & CSS3** (Responsive design con Glassmorphism)

---

## 💻 Ejecución en Local

Si deseas clonar y ejecutar este proyecto en tu propia máquina:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/Ingeep/3d-threejs.git
   cd 3d-threejs
   ```

2. Debido a las políticas de seguridad CORS de los navegadores para texturas locales, inicia un servidor web local:
   ```bash
   # Con Python:
   python -m http.server 8000
   ```
   *(O usando la extensión **Live Server** en VS Code).*

3. Abre en tu navegador:
   ```text
   http://localhost:8000
   ```

---

## 👤 Autor

* **Oseas I. Pozo Almonte**
* GitHub: [@Ingeep](https://github.com/Ingeep)
