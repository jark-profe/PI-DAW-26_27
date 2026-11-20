# 🚀 Checkpoint 4: Prueba de Concepto (PoC)

En esta fase pasamos del diseño al código. El objetivo de la **Prueba de Concepto (PoC)** es demostrar con un prototipo funcional mínimo que **el núcleo principal de tu aplicación** funciona de extremo a extremo (**Frontend ➔ Backend ➔ Base de Datos / API externa**).

---

## 📋 ¿Qué debes entregar en este Checkpoint?

### 1. Código base en el repositorio
El proyecto debe estar subido a GitHub con una estructura de carpetas ordenada y limpia (recuerda configurar bien el `.gitignore` para no subir `node_modules/`, `vendor/` o archivos `.env` con contraseñas reales).

### 2. El flujo principal de tu negocio (Core End-to-End)
No se trata de hacer un simple login o registro genérico, sino de programar **la funcionalidad clave que define tu aplicación** y que conlleva su mayor reto técnico:
* **Frontend:** La interfaz principal de interacción (ej. el mapa con marcadores, el calendario de reservas, el buscador con filtros o el panel de incidencias).
* **Backend:** La lógica o endpoint que procesa la acción principal.
* **Persistencia / API:** Lectura o escritura real en la base de datos de la entidad principal de tu negocio (ej. cargar restaurantes desde la BD y pintarlos en el mapa, guardar una reserva real comprobando disponibilidad, o registrar una incidencia en la comunidad).

---

## 📤 Evidencias a incluir en el `README.md`

Para evaluar este Checkpoint deberás actualizar el `README.md` de tu repositorio incluyendo:

1. **Capturas de pantalla:** Imágenes de la aplicación funcionando en el navegador mostrando la funcionalidad clave junto a la evidencia de los datos en la base de datos.
2. **Vídeo-demo (máx. 2-3 minutos):** Un vídeo breve (subido a YouTube en oculto, Google Drive o enlazado en el README) donde enseñes tu pantalla, muestres brevemente la estructura del código y ejecutes en directo el flujo principal de tu PoC explicando cómo funciona.
