# 📌 Guía para definir los Roles

1. **Rol An&oacute;nimo:** Representa al usuario no autenticado (visitante público). Solo puede acceder a vistas públicas.
2. **Rol de Usuario Registrado:** Usuarios que se dan de alta, generalmente mediante un formulario público de registro (Sign Up). Una vez autenticado en la aplicación, podrá tener acceso a ciertas vistas privadas acotadas según su rol.
3. **Rol de Administrador:** Rol con privilegios globales sobre la plataforma. NO dispone de formulario de registro público. Sus credenciales se generan por defecto, siendo obligatorio el cambio de contraseña tras el primer acceso. Una vez autenticado, tendrá acceso a vistas administrativas.

---

# 📌 Guía para definir los Requisitos Funcionales (RF)

Vamos a distinguir entre los RF de un usuario y los RF del sistema (`RF-SYS`):

1. **Requisitos de usuario (`RF`):** Aqui definimos qué puede hacer un usuario con cierto rol.
2. **Requisitos del Sistema (`RF-SYS`):** Funcionalidades, automatismos o reglas de negocio que ejecuta la aplicación en segundo plano, sin requerir una acción explícita por parte de ningún usuario.

---

# 📝 Ejemplos: Definición de Roles y Requisitos Funcionales (RF)

## 1️⃣ Caso 1: GymFlex

* **Tipo:** Gestión de reservas  
* **Área:** Salud y deporte (Gimnasio local)  
* **Descripción:** Aplicación web para un gimnasio de barrio que permite a los socios consultar la disponibilidad de clases dirigidas (Spinning, Yoga, Pilates), reservar su plaza con antelación y cancelar si no pueden asistir. Además, los entrenadores pueden consultar la lista de asistentes a sus clases y la gerencia puede gestionar el catálogo de actividades, horarios, salas y entrenadores.

### 👥 Roles
* **Anónimo:** Visitante público no autenticado.
* **Socio:** Cliente del centro con suscripción activa.
* **Entrenador:** Empleado encargado de impartir las clases.
* **Gerente (Admin):** Personal de gestión global del centro deportivo.

### ⚙️ Ejemplos de algunos Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-01** | Anónimo | Consultar la parrilla semanal de actividades, horarios, entrenadores y aforo libre en tiempo real. |
| **RF-02** | Anónimo | Visualizar tarifas de suscripción, galería de instalaciones y ubicación del centro. |
| **RF-03** | Socio | Reservar plaza en una clase dirigida si existe aforo disponible. |
| **RF-04** | Socio | Cancelar una reserva previa dentro del plazo límite establecido por el centro. |
| **RF-05** | Entrenador | Consultar la lista actualizada de socios inscritos en sus clases asignadas del día. |
| **RF-06** | Administrador | Crear, editar, consultar o cancelar salas, actividades y sesiones de entrenamiento. |
| **RF-07** | Administrador | Dar de alta, consultar perfil, modificar datos, o dar de baja a los entrenadores. |
| **RF-SYS-01** | Sistema | Habilitar automáticamente la reserva de cada clase 48 horas antes de su horario de inicio. |
| **RF-SYS-02** | Sistema | Promocionar automáticamente al primer socio en lista de espera cuando se registra una cancelación. |

---

## 2️⃣ Caso 2: EcoMarket

* **Tipo:** Tienda online (E-commerce)  
* **Área:** Comercio local y sostenible  
* **Descripción:** Plataforma de e-commerce que permite a pequeños productores locales vender frutas, verduras y productos artesanos directamente al consumidor final. Los clientes pueden explorar el catálogo por categorías, añadir productos a la cesta, gestionar su dirección de envío y realizar el pedido. Los productores pueden actualizar el stock de sus productos y ver los pedidos recibidos, mientras que el administrador supervisa las comisiones y valida el alta de nuevos vendedores.

### 👥 Roles
* **Anónimo:** Cliente o vendedor potencial.
* **Cliente:** Comprador registrado en la plataforma.
* **Vendedor:** Proveedor que oferta sus productos locales.
* **Administrador:** Gestor global de la plataforma e-commerce.

### ⚙️ Ejemplos de algunos Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-01** | Anónimo | Buscar, filtrar por categoría/precio y consultar fichas públicas de productos y productores. |
| **RF-02** | Anónimo | Añadir y modificar productos dentro de un carrito de compra temporal almacenado en sesión local. |
| **RF-03** | Cliente | Tramitar el pedido introduciendo la dirección de entrega, método de pago y confirmando la compra. |
| **RF-04** | Cliente | Consultar el historial personal y el estado de seguimiento de sus pedidos (En preparación, Enviado, Entregado). |
| **RF-05** | Vendedor | Registrar nuevos productos, modificar precios, subir imágenes o retirar productos de su catálogo. |
| **RF-06** | Administrador | Validar, aprobar o rechazar las solicitudes de alta de nuevos productores locales. |
| **RF-SYS-01** | Sistema | Descontar automáticamente las unidades del stock disponible tras la confirmación de pago del pedido. |
| **RF-SYS-02** | Sistema | Calcular la comisión correspondiente para la plataforma y el desglose de IVA al cerrar cada transacción. |

---

## 3️⃣ Caso 3: HuertoUrbano (Gestión de parcelas y comunidad)
* **Tipo:** Plataforma comunitaria
* **Área:** Sostenibilidad y agricultura comunitaria
* **Descripción:** HuertoUrbano es una plataforma web orientada a fomentar la agricultura sostenible y la comunidad vecinal mediante la digitalización de un huerto municipal. El sistema permite a los ciudadanos registrarse para consultar el calendario público y solicitar formalmente la asignación de parcelas libres controladas por el ayuntamiento. Además de administrar el espacio físico, la aplicación funciona como un punto de encuentro virtual donde los hortelanos pueden publicar anuncios para el préstamo de herramientas agrícolas e inscribirse en talleres formativos organizados por el coordinador del recinto, creando así un ecosistema colaborativo.

### 👥 Roles
* **Anónimo:** Visitante público.
* **Hortelano:** Usuario registrado con perfil activo.
* **Administrador:** Coordinador municipal del espacio.

### ⚙️ Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-01** | Anónimo | El Anónimo puede consultar los talleres programados en el calendario público. |
| **RF-02** | Hortelano | El Hortelano puede solicitar la asignación de una parcela libre. |
| **RF-03** | Hortelano | El Hortelano puede publicar anuncios en el tablón para prestar herramientas. |
| **RF-04** | Hortelano | El Hortelano puede inscribirse en los talleres publicados. |
| **RF-05** | Admin | El Administrador puede asignar una parcela vacante a la solicitud de un Hortelano. |
| **RF-06** | Admin | El Administrador puede eliminar los anuncios del tablón que incumplan las normas. |
| **RF-SYS-01** | Sistema | El sistema deberá cambiar el estado de un anuncio a "caducado" cuando transcurran 30 días desde su publicación. |
| **RF-SYS-02** | Sistema | El sistema deberá enviar un email de confirmación al Hortelano cuando el Administrador le asigne una parcela. |

---

## 4️⃣ Caso 4: FixIt Desk

* **Tipo:** Gestión interna  
* **Área:** Mantenimiento e incidencias corporativas  
* **Descripción:** Sistema de gestión interna de incidencias técnicas y de mantenimiento para las instalaciones de una organización. Permite a los empleados reportar averías (equipos informáticos, mobiliario, climatización), categorizarlas por urgencia y hacer seguimiento de su resolución. Los técnicos de mantenimiento reciben los partes, cambian el estado de las tareas y asignan prioridades. El responsable de infraestructura supervisa el rendimiento del equipo y gestiona los recursos asignados.

### 👥 Roles
* **Anónimo:** Usuario no autenticado en la red interna.
* **Empleado:** Personal de la organización que reporta incidencias.
* **Técnico de mantenimiento:** Operario encargado de resolver las averías asignadas.
* **Responsable de infraestructuras (Admin):** Gestor del servicio, reparto de cargas y análisis de métricas.

### ⚙️ Ejemplos de algunos Requisitos Funcionales (RF)

| Código | Rol | Descripción del Requisito |
| :--- | :--- | :--- |
| **RF-01** | Anónimo | Acceder a la pantalla de autenticación (Login) y consultar una guía (FAQ) pública de soporte. |
| **RF-02** | Empleado | Registrar un nuevo parte de incidencia indicando ubicación, tipo de avería, descripción y nivel de urgencia. |
| **RF-03** | Empleado | Consultar el estado actualizado de sus partes registrados (Pendiente, En Proceso, Resuelto). |
| **RF-04** | Técnico | Actualizar la fase del parte asignado e incluir observaciones técnicas sobre la reparación realizada. |
| **RF-05** | Administrador | Asignar o derivar manualmente partes de incidencias entre técnicos y modificar prioridades. |
| **RF-SYS-01** | Sistema | Asignar automáticamente el parte al área técnica correspondiente según la categoría seleccionada. |
| **RF-SYS-02** | Sistema | Enviar una notificación automática (email/interna) al empleado cuando el estado de su incidencia se actualice. |

---

### 🚩 Errores comunes al redactar Requisitos Funcionales (y cómo evitarlos)

Para que los Requisitos Funcionales (RF) sean útiles y os sirvan de guía para diseñar la base de datos más adelante, deben ser precisos, medibles y no dejar nada a la imaginación. 

Aquí tenéis los 3 errores más clásicos que suponen un "No Apto":

#### 1. Requisitos vagos o imprecisos (El "verbo trampa")
Los verbos genéricos como "gestionar", "administrar" o "comprar" ocultan muchas acciones y no nos dicen qué datos hay que guardar. Hay que desglosar la acción real.
* ❌ **Mal:** *"RF-01: El usuario puede comprar cosas en la web."*
* ✅ **Bien:** *"RF-01: El usuario Cliente puede añadir, modificar la cantidad y eliminar productos de su carrito de la compra."*
> 💡 *Por qué importa:* El requisito bien escrito ya te sugiere exactamente qué entidades vas a necesitar modelar luego (`Cliente`, `Producto`, `Carrito`).

#### 2. Olvidar los roles y permisos (El "requisito fantasma")
Si una acción no dice **quién** la ejecuta, es un error de diseño. No todos los usuarios pueden hacer de todo en un sistema real.
* ❌ **Mal:** *"RF-02: Se podrán borrar los comentarios del foro."* (¿Quién? ¿Un invitado? ¿Cualquiera?)
* ✅ **Bien:** *"RF-02: El usuario con rol 'Autor' puede borrar sus propios comentarios, y el 'Administrador' puede borrar los de cualquier persona."*
> 💡 *Por qué importa:* Te obliga a tener en cuenta la tabla de `Roles` o `Permisos` desde el principio y evita fallos graves de seguridad en la aplicación.

#### 3. Mezclar diseño (UI) con funcionalidad (Backend)
El Análisis define **QUÉ** hace el sistema, no **CÓMO** se ve o implementa. Guardad los colores, los botones y la maquetación para la fase de Diseño.
* ❌ **Mal:** *"RF-03: Habrá un menú lateral azul con un botón grande para ver el perfil."*
* ✅ **Bien:** *"RF-03: El sistema permitirá al usuario registrado consultar y actualizar los datos de su perfil personal (nombre, email y contraseña)."*
> 💡 *Por qué importa:* La interfaz puede cambiar 20 veces (web, móvil, escritorio), pero el requisito de negocio y los datos del perfil siguen siendo los mismos.
