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

*(Continuará...)*
