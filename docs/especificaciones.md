# Especificaciones del Proyecto: Wedding Landing Page - "Recuerdos Inolvidables"

## 1. Objetivo del Producto
Crear una experiencia digital de transición (puente) elegante y ágil para los invitados de la boda de **Abdiel & Abigahil**. El sitio debe motivar a los usuarios a compartir su contenido multimedia (fotos y videos) del evento de manera sencilla tras escanear un código QR físico en el lugar del evento.

## 2. Flujo del Usuario (User Journey)
1. **Acceso:** El invitado escanea un código QR en una tarjeta física o cartel de mesa.
2. **Aterrizaje:** El usuario llega a la landing page optimizada para dispositivos móviles.
3. **Interacción:** El usuario lee el mensaje de agradecimiento y visualiza la estética editorial del evento.
4. **Conversión:** El usuario hace clic en el botón principal "Compartir Fotografía o Video".
5. **Salida:** El sistema redirige automáticamente a la URL externa de Knipsmig: `https://knipsmig.com/Z3749o5k`.

## 3. Arquitectura de Información (Estructura de la Página)

### A. Header (Fijo/Glassmorphism)
* **Logotipo/Identidad:** Texto "Abdiel & Abigahil" en tipografía *Noto Serif* (Italic).
* **Iconografía:** Icono de corazón (`favorite`) en color `primary`.
* **Navegación (Desktop):** Enlaces secundarios ("Our Story", "Thank You") con tracking amplio.

### B. Sección Hero (Bienvenida)
* **Badge Superior:** Etiqueta redondeada con el texto "RECUERDOS INOLVIDABLES".
* **Título Principal:** "¡Gracias por acompañarnos!" (H1, Noto Serif, Italic).
* **Bloque de Texto:** Mensaje de agradecimiento enfatizando la alegría de compartir fotos y videos. Debe usar un marco decorativo en 'L' en la esquina superior izquierda.

### C. Call to Action (CTA Principal)
* **Componente:** Botón de gran formato con bordes muy redondeados (píldora).
* **Contenido:** Icono de cámara (`photo_camera`) + Texto "Compartir Fotografía o Video".
* **Comportamiento:** Redirección inmediata a la galería de Knipsmig.

### D. Galería Editorial (Visual Feedback)
* **Distribución:** Grid asimétrico de 2 columnas.
* **Contenido:** 4 espacios para imágenes que representen la estética del evento (flores, momentos románticos, detalles de la recepción).
* **Estilo:** Bordes redondeados (`lg`) y sombras ambientales muy suaves.

### E. Cierre y Firma
* **Firma:** "Con amor, Abdiel & Abigail" en tipografía serif.
* **Iconos Decorativos:** Fila de 3 iconos (`loyalty`, `favorite`, `celebration`) para reforzar el sentimiento festivo.

### F. Footer
* **Contenido:** Repetición de nombres, enlaces de navegación simples y créditos de diseño con el año "2026".

## 4. Requerimientos Técnicos y No Funcionales

### A. Performance & PWA
* **Carga Crítica:** La página debe cargar en menos de 2 segundos en redes 4G/LTE (considerando la cobertura en zonas de eventos en Tapalpa).
* **PWA Ready:** Debe incluir un `manifest.json` y configuración básica para que los invitados puedan "instalar" el acceso directo si así lo desean durante el evento.

### B. Responsividad
* **Mobile-First:** Diseño optimizado para resoluciones de iPhone y Android modernos.
* **Desktop:** Layout centrado y contenido max-width de `lg` (aprox 512px) para mantener la sensación de "invitación vertical".

### C. Accesibilidad
* Contraste mínimo de texto sobre fondo conforme a WCAG 2.1.
* Etiquetas `alt` descriptivas en todas las imágenes de la galería.

## 5. Glosario de Copys (Textos Oficiales)
* **Headline:** "¡Gracias por acompañarnos!"
* **Cuerpo:** "Estamos inmensamente alegres de que quieran compartir este momento tan especial con sus fotos y videos."
* **URL de Destino:** `https://knipsmig.com/Z3749o5k`