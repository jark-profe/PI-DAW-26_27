# 📌 Checkpoint 3: Diseño

En este apartado definiremos aspectos sobre **cómo** vamos a realizar nuestra aplicación.

---

## 📋 ¿Qué debes entregar en este Checkpoint?

### 1. Listado de vistas

Un listado con todas las vistas que compondrán la aplicación, agrupándolas en las siguientes tres categorías:

* **Vistas públicas:** Accesibles para cualquier visitante sin necesidad de autenticación (ej. *Landing page*, formulario de registro, inicio de sesión, términos de servicio, etc).
* **Vistas privadas (Usuario autenticado):** Accesibles únicamente tras iniciar sesión con un rol estándar (ej. perfil de usuario, historial de actividad, panel principal, proceso de pago/reserva, etc).
* **Vistas de gestión (Administración):** Accesibles exclusivamente por usuarios administradores para el control de la plataforma (ej. panel de control / *dashboard*, gestión de usuarios, edición de catálogo, etc).

---

#### 💡 Ejemplo de algunas posibles vistas:

* **Vistas públicas:**
  * `V-01: Inicio` (`/`) — Página principal de presentación.
  * `V-02: Registro` (`/registro`) — Formulario para crear una cuenta.

* **Vistas privadas:**
  * `V-03: Mi perfil` (`/perfil`) — Datos personales y ajustes del usuario.
  * `V-04: Mis pedidos` (`/historial`) — Historial de compras o reservas realizas.

* **Vistas de gestión:**
  * `V-05: Panel de control` (`/admin`) — Panel principal del administrador.
  * `V-06: Gestión de usuarios` (`/admin-usuarios`) — Para dar de alta o baja usuarios registrados.

---

### 2. Mapa de Vistas (Sitemap / Flujo de Navegación)

En este apartado se debe representar de forma visual la estructura de navegación de la aplicación web, mostrando cómo se interconectan las distintas pantallas mediante acciones del usuario.

---

#### 📌 Requisitos de elaboración

1. **Clasificación por roles:** El diagrama debe organizar las vistas en tres bloques o áreas visuales claramente diferenciadas según el nivel de acceso: **Anónimo (Públicas)**, **Usuario registrado (Privadas)** y **Administrador (Gestión)**.
2. **Identificación de las vistas:** Cada nodo del gráfico debe coincidir exactamente con el código y nombre asignado en el listado de vistas anterior (ej. `[V-01] Inicio`).
3. **Flujos y transiciones (flechas):**
   * **Flecha continua (`--->`):** Navegación directa mediante enlaces, botones o menús.
   * **Flecha discontinua (`-.->`):** Redirección condicional del sistema (ej. tras validación de credenciales en la vista de Login).

---

#### 🛠️ Herramientas recomendadas

Se recomienda utilizar cualquiera de las siguientes herramientas para la entrega, pero siempre dejar al menos una imagen para que yo pueda verla:

* **Mermaid.js:** Permite renderizar el diagrama mediante código dentro de archivos `.md` de GitHub.*
* * **Draw.io:** Herramienta gratuita sin registro obligatorio. Permite estructurar el mapa por contenedores y exportar la imagen (`.png` / `.svg`).
* **Miro / FigJam / Canva:** Lienzos interactivos ideales para diseñar esquemas mediante componentes *drag-and-drop*.

---

#### 💡 Ejemplo en Mermaid.js
<img width="670" height="745" alt="image" src="https://github.com/user-attachments/assets/af189880-2993-42e8-ba05-2d54cdfba162" />

---

### 3. Prototipado de fidelidad <ins>media</ins> (Figma)

En este apartado se debe presentar el diseño visual estructural (*wireframes*) de las pantallas definidas en el listado de vistas, utilizando **Figma** como herramienta principal.

---

#### 📌 Requisitos de elaboración

1. **Correspondencia con el inventario:** Deben diseñarse todas las vistas catalogadas en el punto 1 (`V-01`, `V-02`, etc.), identificando cada marco (*Frame*) de Figma con su código y nombre correspondiente.
2. **Fidelidad media:** Los diseños deben mostrar una estructura clara de componentes, jerarquía visual, distribución de espacios (*layout*), menús de navegación, formularios y textos reales o representativos (evitando abusar del *Lorem Ipsum*). No es obligatorio aplicar la paleta de colores definitiva ni imágenes finales, pero sí definir claramente la estructura de interfaz (*UI*).
3. **Diseño adaptable (*Responsive*):** Se deberá incluir al menos el diseño de las vistas principales (como mínimo la página de inicio y una vista privada) adaptadas a versión **escritorio (*Desktop*)** y **móvil (*Mobile*)**.

---

#### 📤 Formato de entrega

* **Enlace público:** Incluir en el `README.md` el enlace directo al archivo de Figma con permisos de lectura activados (*"Anyone with the link can view"*).
* **Capturas de respaldo:** Incluir en el `README.md` al menos 2 o 3 capturas de pantalla de las vistas más representativas del proyecto para su previsualización directa en GitHub.

---

### 4. Tecnologías elegidas para el proyecto

En este apartado se detallará y justificará el *stack* tecnológico seleccionado para desarrollar la aplicación, abarcando tanto la parte cliente como la parte servidor y herramientas auxiliares.

---

#### 📌 Requisitos de elaboración

No basta con enumerar las herramientas. Además hay que **justificar brevemente el porqué de cada elección** (curva de aprendizaje, adecuación al proyecto, rendimiento, soporte, etc.) estructurándolo en las siguientes categorías:

* **Frontend (Interfaz y lógica de cliente):** Lenguajes, *frameworks* o librerías CSS/JS (ej. *HTML5, CSS3, Tailwind CSS, Bootstrap, JavaScript, React, Vue, Angular...*).
* **Backend (Lógica de servidor):** Lenguaje y entorno o *framework* de servidor (ej. *PHP, Laravel, Symfony, Node.js, Express, Python, Django, Java, Spring Boot...*).
* **Base de datos:** Sistema gestor de bases de datos seleccionado (ej. *MySQL, MariaDB, PostgreSQL, MongoDB, Firebase...*).
* **APIs externas y librerías adicionales:** Servicios de terceros o librerías específicas que aporten funcionalidad extra al proyecto (ej. *Leaflet.js para mapas, Stripe para pagos, Chart.js para gráficas, PDF.js, etc.*).
* **Entorno de desarrollo y despliegue:** Herramientas de control de versiones, contenedores o alojamiento previstas (ej. *Git/GitHub, Docker, Vercel, Render, Railway, InfinityFree...*).

---

#### 💡 Ejemplo de tabla resumen

| Capa / Área | Tecnología elegida | Justificación |
| :--- | :--- | :--- |
| **Frontend** | HTML5, Tailwind CSS, JavaScript | Permite un maquetado rápido, *responsive* y sin sobrecargar el proyecto con un *framework* complejo. |
| **Backend** | PHP 8 / Laravel | Facilita la arquitectura MVC, gestión segura de rutas, autenticación y consultas mediante Eloquent ORM. |
| **Base de Datos** | MySQL | Motor relacional robusto, idóneo para estructurar usuarios, roles y registros transaccionales. |
| **APIs / Librerías** | Leaflet.js + OpenStreetMap | Solución gratuita y ligera para mostrar ubicaciones interactivas sin depender de cuotas de pago. |
| **Despliegue** | GitHub + Docker / Render | Control de versiones integrado y facilidad para levantar el entorno de producción en la nube. |
