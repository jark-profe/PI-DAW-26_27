# Condiciones y requisitos mínimos del Proyecto Intermodular

¡Bienvenidos a la fase de desarrollo de vuestro Proyecto Intermodular de 2º de DAW! 

El objetivo de este proyecto es integrar todos los conocimientos que habéis adquirido a lo largo de los diferentes módulos del ciclo (Servidor, Cliente, Despliegue, Diseño de Interfaces, etc.). Para asegurar que vuestro proyecto alcanza el nivel exigido para un perfil técnico profesional, hemos establecido una serie de condiciones y requisitos mínimos:

## 1. Requisitos de arquitectura
Estos son los condicionantes estructurales obligatorios que debe cumplir todo proyecto. Representan la base tecnológica de vuestro software:

* **Arquitectura de 3 capas:** El proyecto debe diferenciar de forma clara y estructurada la parte de cliente (Frontend), la de servidor (Backend) y la base de datos.
<img width="608" height="277" alt="image" src="https://github.com/user-attachments/assets/abb5ed51-f421-4f1d-94e2-e2dd0b01e84f" />

* **Despliegue en producción:** La aplicación deberá estar desplegada y plenamente operativa en un servidor de producción (tipo AWS, VPS, Heroku, etc.).
* **Demostración real:** Recordad que durante la exposición final del proyecto se os exigirá realizar la demostración funcional recorriendo una URL en producción, y bajo ningún concepto se admitirá la ejecución en un entorno *localhost*.

## 2. Requisitos Base
Estas son las operativas y características mínimas que debe realizar vuestra aplicación web (el "qué" hace el sistema). 

* **Gestión de Roles:** El sistema debe contar con al menos tres niveles de usuario (Usuario Administrador, Usuario Registrado y Usuario Anónimo).
* **Autenticación:** La aplicación deberá ofrecer un sistema seguro de registro e inicio de sesión para los usuarios (login/logout).
* **Gestión de Perfil:** Todo usuario registrado deberá tener la posibilidad de visualizar y modificar su información de perfil.
* **Gestión de Vistas y Permisos:** El sistema deberá restringir el acceso a la información y a las acciones en función del rol del usuario. 
* **Operaciones CRUD:** La plataforma deberá permitir a los usuarios registrados (según su nivel de permisos) crear, listar, editar y borrar los elementos principales de información del sistema.
📝 **Nota:** Estos requisitos deberán adaptarse y plasmarse en la lista de Requisitos Funcionales de vuestra aplicación. No copiéis y peguéis esta lista en vuestra entrega. Deberéis tomar esta base y **redactarla adaptándola a los usuarios de vuestro proyecto**.

---

💡 **Consejo:** *Un buen proyecto no es el que tiene infinitas funcionalidades a medio terminar, sino el que implementa unas funcionalidades clave de manera robusta, segura y bien estructurada. Empezad siempre por definir bien vuestro MVP (Producto Mínimo Viable).* 
