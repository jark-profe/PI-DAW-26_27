# Condiciones y requisitos mínimos del Proyecto Intermodular

¡Bienvenidos a la fase de desarrollo de vuestro Proyecto Intermodular de 2º de DAW! 

El objetivo de este proyecto es integrar todos los conocimientos que habéis adquirido a lo largo de los diferentes módulos del ciclo (Servidor, Cliente, Despliegue, Diseño de Interfaces, etc.). Para asegurar que vuestro proyecto alcanza el nivel exigido para un perfil técnico profesional, hemos establecido una serie de condiciones y requisitos mínimos innegociables.

Es fundamental que comprendáis que estos requisitos se dividen en tres categorías distintas. Leedlas con atención, ya que os ayudarán a estructurar correctamente vuestra memoria técnica.

## 1. Requisitos técnicos y de arquitectura (Reglas del proyecto)
Estos son los condicionantes estructurales obligatorios que debe cumplir todo proyecto. Representan la base tecnológica de vuestro software:

* **Arquitectura de 3 capas:** El proyecto debe diferenciar de forma clara y estructurada la parte de cliente (Frontend), la de servidor (Backend) y la base de datos.
* **Despliegue en producción:** La aplicación deberá estar desplegada y plenamente operativa en un servidor de producción (tipo AWS, VPS, Heroku, etc.).
* **Demostración real:** Recordad que durante la exposición final del proyecto se os exigirá realizar la demostración funcional recorriendo una URL en producción, y bajo ningún concepto se admitirá la ejecución en un entorno *localhost*.

## 2. Requisitos NO Funcionales (Atributos de calidad)
Hacen referencia a cómo debe comportarse el sistema (rendimiento, usabilidad, seguridad, etc.). 

⚠️ **IMPORTANTE para el Checkpoint de Análisis:** Tal y como se ha indicado en las directrices del ciclo de vida del proyecto, en vuestra entrega de la fase de Análisis NO hay que especificar los Requisitos no funcionales. Debéis cumplirlos técnicamente de cara a aprobar el proyecto, pero no documentarlos en esa fase.
* **Diseño *Responsive*:** La interfaz de la aplicación web deberá ser completamente adaptable a dispositivos móviles y tablets. Tened en cuenta que se os exigirá una demostración de maquetación *responsive* durante vuestra defensa oral ante el tribunal.

## 3. Requisitos Funcionales Base (El "Core" obligatorio)
Estas son las operativas y características mínimas que debe realizar vuestra aplicación web (el "qué" hace el sistema). 

📝 **Nota para la redacción:** No copiéis y peguéis esta lista en vuestra entrega. Deberéis tomar esta base y **redactarla adaptándola a la temática de vuestro proyecto**.
* **Gestión de Roles:** El sistema exige la identificación explícita de los roles, debiendo contar con al menos tres niveles de usuario (ej: Usuario Administrador, Usuario Registrado y Usuario Anónimo).
* **Autenticación:** La aplicación deberá ofrecer un sistema seguro de registro e inicio de sesión para los usuarios.
* **Gestión de Perfil:** Todo usuario registrado deberá tener la posibilidad de visualizar y modificar su información de perfil.
* **Gestión de Vistas y Permisos:** El sistema deberá restringir el acceso a la información y a las acciones en función del rol del usuario. Deberéis definir un listado de URLs clasificadas por su nivel de acceso (vistas públicas, privadas y de gestión).
* **Operaciones CRUD:** La plataforma deberá permitir a los usuarios registrados (según su nivel de permisos) crear, listar, editar y borrar los elementos principales de información (entidades) del sistema.

---

💡 **Consejo:** *Un buen proyecto no es el que tiene infinitas funcionalidades a medio terminar, sino el que implementa unas funcionalidades clave de manera robusta, segura y bien arquitecturada. Empezad siempre por definir bien vuestro MVP (Producto Mínimo Viable).* ¡Mucho ánimo con el desarrollo!
