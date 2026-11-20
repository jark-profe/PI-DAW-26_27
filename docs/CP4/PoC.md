# 🚀 Checkpoint 4: Prueba de Concepto (PoC)

En esta fase pasamos del diseño al código. El objetivo de la **Prueba de Concepto (PoC)** es demostrar con un prototipo funcional mínimo que **el núcleo principal de tu aplicación** funciona de extremo a extremo (**Frontend ➔ Backend ➔ Base de Datos / API externa**).

---

## 📋 ¿Qué debes construir?

No se trata de hacer un simple login o registro genérico, sino de programar **la funcionalidad clave que define tu aplicación** y que conlleva su mayor reto técnico:

* **Frontend:** La interfaz principal de interacción (ej. el mapa con marcadores, el calendario de reservas, el buscador con filtros o el panel de incidencias).
* **Backend:** La lógica o endpoint que procesa la acción principal.
* **Persistencia / API:** Lectura o escritura real en la base de datos de la entidad principal de tu negocio (ej. cargar restaurantes desde la BD y pintarlos en el mapa, guardar una reserva real comprobando disponibilidad, o registrar una incidencia en la comunidad).

---

## 📤 Qué y cómo debes entregarlo

Para dar por superado este Checkpoint, tu repositorio en GitHub debe contener:

1. **Código fuente en la carpeta `/poc`:** Todo el código de esta prueba debe ir alojado dentro de una carpeta llamada `/poc` en la raíz de tu repositorio (así no interferirá cuando empieces a desarrollar la aplicación definitiva). Recuerda configurar bien el `.gitignore` para no subir `node_modules/`, `vendor/` o archivos `.env` con contraseñas reales.
2. **Evidencias en el `README.md`:** Actualiza el `README.md` (o crea un `README.md` dentro de `/poc`) incluyendo:
   * **Capturas de pantalla:** Imágenes (las justas) de la aplicación funcionando en el navegador mostrando la funcionalidad clave junto a la evidencia de los datos en la base de datos.
   * **Vídeo-demo (máx. 3-4 minutos):** Enlace a un vídeo breve (subido a YouTube en oculto o Google Drive) donde enseñes tu pantalla, muestres brevemente la estructura del código y ejecutes en directo el flujo principal de tu PoC explicando cómo funciona.
