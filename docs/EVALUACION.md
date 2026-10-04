## 📊 Evaluación

La calificación final del proyecto se divide en tres bloques principales: **Proyecto (70%)**, **Documentación (20%)** y **Exposición (10%)**.

| Bloque | Subbloque | Peso % | A evaluar |
| :--- | :--- | :---: | :--- |
| **Proyecto** *(70%)* | **Interfaz** | **20%** | • Interfaz responsive.<br>• Coherencia del sistema de diseño en paleta de colores, accesibilidad y jerarquía tipográfica.<br>• Elección, usabilidad y cohesión visual de los componentes a lo largo de las páginas. |
| | **Funcionalidad frontend (Cliente)** | **20%** | • Implementación de vistas públicas, privadas y de perfil, garantizando la protección de rutas y la persistencia de sesión por rol.<br>• Funcionamiento de formularios (registro, login, ver/editar perfil y CRUD) con validación en tiempo real y feedback claro al usuario.<br>• Gestión de estado, modularidad de componentes reusables, navegación/paginación y control de estados de carga/error. |
| | **Funcionalidad backend (Servidor)** | **20%** | • Operaciones CRUD completas y optimizadas sobre la base de datos, con correcta gestión de relaciones, integridad referencial y validación estricta de datos de entrada.<br>• Mecanismo seguro de autenticación y gestión de sesiones (login/logout, almacenamiento seguro de tokens/cookies, hash de contraseñas y expiración/renovación).<br>• Control de acceso basado en roles y uso adecuado de códigos de respuesta HTTP (401, 403, 404, etc). |
| | **Despliegue** | **10%** | • Aplicación está desplegada en un servidor o plataforma cloud accesible públicamente vía URL única.<br>• La aplicación utiliza un certificado SSL/TLS válido (HTTPS) en todo el dominio. <br>•Todos los servicios (Frontend, Backend y BBDD) están correctamente containerizados. El repositorio incluye un Dockerfile optimizado y/o docker-compose.yml que levanta la pila completa sin errores. |
| **Documentación** *(20%)* | **Anteproyecto** | **10%** | [ANTEPROYECTO](ANTEPROYECTO.md) |
| | **Documentación Final** | **5%** | Redacción completa del `README.md` del repositorio cubriendo todas las secciones requeridas. [ENTREGA](ENTREGA.md) |
| | **Seguimiento** | **5%** | Bitácora actualizada semanalmente durante el seguimiento y control de commits en Github, tal como se indica en [DESARROLLO](DESARROLLO.md) |
| **Exposición** *(10%)* | **Exposición** | **10%** | • Correcto uso de los tiempos, lenguaje técnico y expresión oral.<br>• Explicación de la arquitectura y justificación de las decisiones tomadas en cada parte (interfaz, frontend, backend, despliegue).<br>• Demostración realizada en entorno real de producción (no localhost).<br>• Verificación de autoría respondiendo correctamente a las preguntas del tribunal. |

---

## ⚠️ Condiciones obligatorias de evaluación (Requisitos mínimos)

Para que el Proyecto Intermodular pueda ser evaluado y promediado, es **imprescindible** cumplir con los siguientes requisitos mínimos:

1. **Apto en el anteproyecto:**  
   Es condición obligatoria obtener la calificación de **APTO** en la entrega del Anteproyecto para poder continuar con el desarrollo.  
   * **Mecanismo de subsanación:** Si la entrega final del Anteproyecto obtiene la calificación de **NO APTO**, el alumnado recibirá un listado detallado con las correcciones requeridas y dispondrá de un **plazo estricto de una 1 semana** para subsanarlo y conseguir el **APTO**.

2. **Corte del 50% por subbloque (Un 5 sobre 10 mínimo):**  
   El alumnado debe alcanzar como mínimo el **50% de la puntuación asignada en cada uno de los subbloques evaluables** de forma independiente (Interfaz, Frontend, Backend, Lógica de Negocio, Despliegue, Documentación Final y Exposición).

> 🚫 **Consecuencia del incumplimiento:** Si el Anteproyecto no alcanza el APTO tras el periodo de subsanación, o si alguno de los subbloques individuales queda por debajo del 50% de su nota, **la asignatura se considerará suspensa** y se deberá recuperar en el periodo correspondiente.

---
