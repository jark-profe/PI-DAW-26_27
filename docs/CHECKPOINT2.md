# 📌 Checkpoint 2: Análisis

¡Bienvenidos al segundo hito del Proyecto Intermodular! Una vez validada la definición de vuestro proyecto, entramos en la fase de **Análisis**. Aquí responderemos a la pregunta clave: **¿QUÉ debe hacer nuestra aplicación web?**

En esta fase no nos preocupa aún cómo se programará o qué tecnologías usaremos, sino detallar con precisión las operativas, los usuarios que interactuarán con la aplicación y las pantallas o vistas que necesitarán.

---

## 📋 ¿Qué debes entregar en este Checkpoint?

En la sección correspondiente al Checkpoint 2 de tu documentación en GitHub, deberás incluir obligatoriamente estos 3 apartados:

### 1. Requisitos Funcionales (RF)
Listado numerado y explicativo de todas las acciones, características y funcionalidades que el sistema debe permitir realizar.
* **Formato:** Cada requisito debe tener un código identificador (ej: `RF-01`, `RF-02`), un título claro y una breve explicación de qué permite hacer.
* ⚠️ **REGLA OBLIGATORIA:** **NO incluyas Requisitos No Funcionales** (rendimiento, tiempos de respuesta, tecnología a usar, etc.). Enfócate únicamente en las funcionalidades que usa el usuario.

### 2. Identificación de Roles
Definición  de los diferentes tipos de usuarios que interactuarán con la plataforma y qué permisos generales tiene cada uno.
* ⚠️ **REGLA OBLIGATORIA:** La aplicación debe contar con **al menos 3 roles diferenciados** (por ejemplo: *Usuario Anónimo*, *Usuario Registrado / Cliente* y *Administrador / Gestor*).

### 3. Mapa de Vistas (Estructura de URLs)
Listado ordenado de las rutas/URLs de la aplicación web, agrupadas según su nivel de acceso.
Deberás clasificar las vistas en tres categorías:
* **Vistas Públicas:** Accesibles por cualquier visitante sin necesidad de autenticarse (ej: `/`, `/login`, `/registro`, `/catalogo`).
* **Vistas Privadas:** Accesibles solo para usuarios autenticados (ej: `/perfil`, `/mis-reservas`, `/carrito`).
* **Vistas de Administración:** Accesibles únicamente por roles con privilegios elevados (ej: `/admin/dashboard`, `/admin/usuarios`, `/admin/productos/crear`).

---

## ⛔ Errores frecuentes que causan un "NO APTO"

Asegúrate de revisar estos puntos antes de realizar tu entrega:

* **Incluir Requisitos No Funcionales:** Escribir requisitos como *"La base de datos será MySQL"* o *"La web tardará menos de 2 segundos en cargar"*. Eso NO pertenece al análisis funcional.
* **Tener menos de 3 roles:** Proponer un sistema donde solo exista un rol o no se diferencie entre un visitante anónimo y un usuario registrado.
* **Requisitos vagos o imprecisos:** Usar frases genéricas como *"RF-01: El usuario puede hacer movidas guapas en la web"*. Sé concreto (ej: *"RF-01: El usuario anónimo puede registrarse mediante correo y contraseña"*).
* **Rutas incoherentes:** Listar URLs que no corresponden a una aplicación web real o no clasificarlas por nivel de acceso.

---

## 💡 Ejemplos de redacción correcta

### Ejemplo de Requisitos Funcionales (RF):
* **`RF-01` — Registro de usuarios:** El sistema permitirá a usuarios anónimos registrarse proporcionando nombre, email y contraseña.
* **`RF-02` — Gestión de productos (CRUD):** El administrador podrá crear, listar, editar y eliminar productos del catálogo.
* **`RF-03` — Búsqueda y filtrado:** El usuario cliente podrá buscar productos a través de texto y filtrarlos por categoría y rango de precio.

### Ejemplo de Clasificación de Vistas:
* **Públicas:**
  * `/` — Página principal de bienvenida.
  * `/login` — Formulario de inicio de sesión.
  * `/registro` — Formulario de alta de usuario.
* **Privadas:**
  * `/perfil` — Consulta y edición de datos personales.
  * `/pedidos` — Historial de pedidos realizados por el usuario.
* **Gestión:**
  * `/admin/dashboard` — Métricas generales y panel principal.
  * `/admin/productos` — Listado y gestión CRUD de productos.
