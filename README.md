📰 Nexus | Noticias

Una aplicación web moderna y minimalista para leer noticias de ciberseguridad y tecnología, con un diseño responsive que se adapta a todos los dispositivos.

✨ Características

· Interfaz Dual: Tema claro y oscuro configurable
· Gestión Local: Sistema de favoritos que se guarda en tu navegador
· Búsqueda Avanzada: Filtra noticias por categoría o palabras clave
· Notificaciones: Panel de alertas con contador de no leídas
· Estadísticas: Seguimiento de tu actividad de lectura
· Carga Rápida: Caché inteligente para mejor rendimiento
· Totalmente Responsive: Diseño optimizado para móviles y escritorio

🚀 Despliegue en Netlify

Esta aplicación está configurada para desplegarse automáticamente en Netlify.

Para desplegar manualmente:

1. Ve a app.netlify.com
2. Haz clic en "Add new site" → "Import an existing project"
3. Conecta tu cuenta de GitHub y selecciona este repositorio
4. Configuración de compilación:
   · Build command: (dejar vacío)
   · Publish directory: (dejar vacío)
5. Haz clic en "Deploy site"

Despliegue continuo

· Cada vez que actualices los archivos JSON (noticias.json o notificaciones.json) y los subas a GitHub, Netlify reconstruirá y desplegará automáticamente la versión actualizada.

📁 Estructura del Proyecto

```
/
├── index.html          # Aplicación principal (HTML, CSS y JS embebidos)
├── noticias.json       # Fuente de datos de noticias
├── notificaciones.json # Datos de alertas y notificaciones
└── README.md           # Este archivo
```

🔧 Cómo Actualizar el Contenido

Actualizar noticias:

1. Edita el archivo noticias.json en GitHub
2. Los cambios deben seguir este formato:

```json
{
  "articles": [
    {
      "id": 1,
      "title": "Título de la noticia",
      "category": "Categoría",
      "date": "Fecha en formato ISO",
      "image": "URL de la imagen",
      "content": "Contenido completo de la noticia...",
      "source": "Fuente de la noticia",
      "excerpt": "Resumen breve"
    }
  ]
}
```

Actualizar notificaciones:

1. Edita el archivo notificaciones.json en GitHub
2. Los cambios deben seguir este formato:

```json
{
  "notifications": [
    {
      "id": 1,
      "title": "Título de la alerta",
      "message": "Mensaje de la notificación",
      "date": "Fecha en formato ISO",
      "read": false
    }
  ]
}
```

🌐 Fuentes de Datos

La aplicación carga contenido dinámico desde:

· https://raw.githubusercontent.com/USUARIO/REPOSITORIO/main/noticias.json
· https://raw.githubusercontent.com/USUARIO/REPOSITORIO/main/notificaciones.json

Nota: Reemplaza USUARIO y REPOSITORIO con tus datos reales en el archivo index.html.

🛠 Tecnologías Utilizadas

· HTML5 - Estructura semántica
· CSS3 - Variables CSS, Flexbox, Grid, diseño responsive
· JavaScript Vanilla - Lógica de la aplicación
· Font Awesome - Iconografía
· GitHub - Almacenamiento de datos y control de versiones
· Netlify - Hospedaje y despliegue continuo

📱 Características Técnicas

· Almacenamiento Local: Usa localStorage para guardar preferencias
· API Fetch: Carga asíncrona de datos desde GitHub
· Diseño Mobile-First: Enfoque responsive desde móviles
· CSS Variables: Para una fácil personalización de temas
· Manejo de Errores: Caché de respaldo si GitHub no está disponible

🔒 Privacidad

Esta aplicación:

· ✅ No recopila datos personales
· ✅ Guarda todo localmente en tu dispositivo
· ✅ No usa cookies de seguimiento
· ✅ No comparte información con terceros

📄 Licencia

© 2025 Nexus Studios.

🙏 Créditos

· Icons: Font Awesome 6.4.0
· Default Images: Unsplash
· Fonts: System UI stack
· Inspiration: Varias aplicaciones de noticias modernas

---

Consejo: Para personalizar la aplicación, edita las variables CSS en la sección :root del archivo index.html para cambiar colores, tamaños y otros aspectos visuales.

¡Disfruta de tu aplicación de noticias! 🚀
