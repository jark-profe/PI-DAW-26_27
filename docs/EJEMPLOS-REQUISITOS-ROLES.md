# 📝 Práctica de Clase: Definición de Roles y Requisitos Funcionales (RF)

**Asignatura:** Proyecto Intermodular — 2º DAW  
**Curso Académico:** 2026 / 2027  
**Objetivo:** Identificar correctamente la taxonomía de roles de usuario y derivar los Requisitos Funcionales (RF) principales, diferenciando entre eventos de interfaz de usuario y Requisitos del Sistema (RF-SYS).

---

## 📌 Guía y Reglas para la Resoluci&oacute;n

1. **Rol An&oacute;nimo (`RF-ANON`):** Representa al usuario no autenticado (visitante público). Tiene permisos estrictamente de **solo lectura (GET)** sobre recursos públicos. Jam&aacute;s realiza operaciones de escritura (`POST`, `PUT`, `DELETE`) ni persiste datos en la base de datos.
2. **Roles Autenticados:** Usuarios registrados en la plataforma con credenciales válidas y permisos acotados según su perfil de negocio.
3. **Requisitos del Sistema (`RF-SYS`):** Funcionalidades, automatismos o reglas de negocio que ejecuta la aplicación en segundo plano (*cron jobs*, eventos de dominio, disparadores) sin requerir una acción explícita por parte de un usuario.

---

## 1️⃣ Caso 1: GymFlex

* **Tipo:** Gestión de Reservas  
* **Área:** Salud y Deporte (Gimnasio Local)  
* **Descripción:** Sistema web para un gimnasio de barrio que permite a los socios consultar la disponibilidad de clases dirigidas (Spinning, Yoga, Pilates), reservar su plaza con antelación y cancelar si no pueden asistir. Además, los entrenadores pueden consultar la lista de asistentes a sus clases y la gerencia puede gestionar el catálogo de actividades, horarios y el aforo máximo de cada sala.

### 👥 Roles del Sistema
* **Anónimo:** Visitante público no autenticado.
* **Socio:** Cliente del centro con suscripción activa.
* **Entrenador / Monitor:** Empleado encargado de impartir las clases.
* **Administrador / Gerente:** Personal de gestión global del centro deportivo.

### ⚙️ Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-ANON01** | Anónimo | Consultar la parrilla semanal de actividades, horarios, entrenadores y aforo libre en tiempo real. |
| **RF-ANON02** | Anónimo | Visualizar tarifas de suscripción, galería de instalaciones y ubicación del centro. |
| **RF01** | Socio | Reservar plaza en una clase dirigida si existe aforo disponible. |
| **RF02** | Socio | Cancelar una reserva previa dentro del plazo límite establecido por el centro. |
| **RF03** | Entrenador | Consultar la lista actualizada de socios inscritos en sus clases asignadas del día. |
| **RF04** | Administrador | Crear, editar o cancelar sesiones en el calendario y definir el aforo máximo por sala. |
| **RF-SYS01** | Sistema | Habilitar automáticamente la reserva de cada clase 48 horas antes de su horario de inicio. |
| **RF-SYS02** | Sistema | Promocionar automáticamente al primer socio en lista de espera cuando se registra una cancelación. |

---

## 2️⃣ Caso 2: EcoMarket

* **Tipo:** Tienda Online (E-commerce)  
* **Área:** Comercio Local y Sostenible  
* **Descripción:** Plataforma de e-commerce que permite a pequeños productores locales vender frutas, verduras y productos artesanos directamente al consumidor final. Los clientes pueden explorar el catálogo por categorías, añadir productos a la cesta, gestionar su dirección de envío y realizar el pedido. Los productores pueden actualizar el stock de sus productos y ver los pedidos recibidos, mientras que el administrador supervisa las comisiones y valida el alta de nuevos vendedores.

### 👥 Roles del Sistema
* **Anónimo:** Visitante o comprador potencial sin sesión iniciada.
* **Cliente:** Comprador registrado en la plataforma.
* **Vendedor / Productor:** Proveedor que oferta sus productos locales.
* **Administrador:** Gestor global de la plataforma e-commerce.

### ⚙️ Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-ANON01** | Anónimo | Buscar, filtrar por categoría/precio y consultar fichas públicas de productos y productores. |
| **RF-ANON02** | Anónimo | Añadir y modificar productos dentro de un carrito de compra temporal almacenado en sesión local. |
| **RF01** | Cliente | Tramitar el pedido introduciendo la dirección de entrega, método de pago y confirmando la compra. |
| **RF02** | Cliente | Consultar el historial personal y el estado de seguimiento de sus pedidos (En preparación, Enviado, Entregado). |
| **RF03** | Vendedor | Registrar nuevos productos, modificar precios, subir imágenes o retirar productos de su catálogo. |
| **RF04** | Administrador | Validar, aprobar o rechazar las solicitudes de alta de nuevos productores locales. |
| **RF-SYS01** | Sistema | Descontar automáticamente las unidades del stock disponible tras la confirmación de pago del pedido. |
| **RF-SYS02** | Sistema | Calcular la comisión correspondiente para la plataforma y el desglose de IVA al cerrar cada transacción. |

---

## 3️⃣ Caso 3: HuertoUrbano

* **Tipo:** Plataforma Comunitaria  
* **Área:** Sostenibilidad y Agricultura Comunitaria  
* **Descripción:** Plataforma web para la comunidad de usuarios de los huertos urbanos municipales. Permite a los vecinos solicitar una parcela de cultivo, organizar talleres formativos y compartir herramientas o consejos agrícolas. Los usuarios pueden publicar eventos, inscribirse en actividades grupales y ofrecer/pedir herramientas prestadas. El coordinador municipal supervisa la asignación de parcelas y modera el tablón de anuncios.

### 👥 Roles del Sistema
* **Anónimo:** Vecino o visitante sin registro en el portal.
* **Hortelano / Vecino:** Usuario registrado activo en la comunidad.
* **Coordinador / Moderador:** Responsable municipal encargado de la supervisión del espacio y las actividades.

### ⚙️ Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-ANON01** | Anónimo | Leer publicaciones del tablón general de avisos y consultar el calendario público de talleres. |
| **RF01** | Hortelano | Enviar una solicitud formal para optar a la asignación de una parcela de cultivo libre. |
| **RF02** | Hortelano | Publicar anuncios para ofrecer o solicitar el préstamo temporal de herramientas agrícolas. |
| **RF03** | Hortelano | Inscribirse a talleres formativos y jornadas de trabajo comunitario programadas. |
| **RF04** | Coordinador | Gestionar la lista de espera y asignar las parcelas vacantes a los solicitantes. |
| **RF05** | Coordinador | Moderar, editar o eliminar publicaciones y comentarios que vulneren las normas de convivencia. |
| **RF-SYS01** | Sistema | Marcar automáticamente como "caducado" un anuncio de préstamo transcurridos 30 días sin actividad. |
| **RF-SYS02** | Sistema | Consolidar automáticamente las solicitudes de talleres aprobadas en la agenda comunitaria del portal. |

---

## 4️⃣ Caso 4: FixIt Desk

* **Tipo:** Gestión Interna  
* **Área:** Mantenimiento e Incidencias Corporativas  
* **Descripción:** Sistema de gestión interna de incidencias técnicas y de mantenimiento para las instalaciones de una organización. Permite a los empleados reportar averías (equipos informáticos, mobiliario, climatización), categorizarlas por urgencia y hacer seguimiento de su resolución. Los técnicos de mantenimiento reciben los partes, cambian el estado de las tareas y asignan prioridades. El responsable de infraestructura supervisa el rendimiento del equipo y gestiona los recursos asignados.

### 👥 Roles del Sistema
* **Anónimo:** Usuario no autenticado en la red interna.
* **Empleado / Solicitante:** Personal de la organización que reporta incidencias.
* **Técnico de Mantenimiento:** Operario encargado de resolver las averías asignadas.
* **Responsable de Infraestructuras (Admin):** Gestor del servicio, reparto de cargas y análisis de métricas.

### ⚙️ Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-ANON01** | Anónimo | Acceder a la pantalla de autenticación (Login) y consultar la base de conocimiento/FAQ pública de soporte. |
| **RF01** | Empleado | Registrar un nuevo parte de incidencia indicando ubicación, tipo de avería, descripción y nivel de urgencia. |
| **RF02** | Empleado | Consultar el estado actualizado de sus partes registrados (Pendiente, En Proceso, Resuelto). |
| **RF03** | Técnico | Actualizar la fase del parte asignado e incluir observaciones técnicas sobre la reparación realizada. |
| **RF04** | Administrador | Asignar o derivar manualmente partes de incidencias entre técnicos y modificar prioridades. |
| **RF-SYS01** | Sistema | Asignar automáticamente el parte al área técnica correspondiente según la categoría seleccionada. |
| **RF-SYS02** | Sistema | Enviar una notificación automática (email/interna) al empleado cuando el estado de su incidencia se actualice. |