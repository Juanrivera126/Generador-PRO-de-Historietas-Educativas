# 🎛 Generador PRO de Historietas Educativas

Una aplicación web profesional para generar historietas educativas usando inteligencia artificial con [Pollinations.ai](https://enter.pollinations.ai/authorize). Crea guiones narrativos completos e imágenes de cómic personalizadas para cualquier tema educativo.

![Version](https://img.shields.io/badge/version-1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## ✨ Características

- 🤖 **Generación de Guiones por Lotes**: Para historietas con más de 10 diapositivas, el guión se genera en lotes preservando la continuidad narrativa
- 🎨 **Múltiples Estilos Visuales**: 30+ estilos incluyendo Pixar, Disney, Anime, Marvel/DC, Studio Ghibli, y más
- 🌐 **Multilingüe**: Soporte completo para Español, English y Français
- 🎭 **Géneros Narrativos**: 25+ géneros desde misterio y superhéroes hasta biografías educativas
- 🗑️ **Gestión de Diapositivas**: Botón de eliminar/restaurar en cada slide para controlar el contenido final
- 📱 **Descargas Flexibles**:
  - 🗂️ ZIP con todas las imágenes
  - 📺 Presentación HTML interactiva
  - 📰 **Tira Cómica HTML**: Página única con grid de 2 columnas y modal para ver imágenes ampliadas
- 🔑 **Integración Pollinations.ai**: Usa tu API Key para generación ilimitada de imágenes

## 🚀 Cómo Usar

1. **Obtén tu API Key**:
   - Visita [Pollinations.ai](https://enter.pollinations.ai/authorize)
   - O usa el botón "Obtener API Key Automáticamente" en la app

2. **Configura tu Historieta**:
   - **Tema Central**: El tema educativo principal
   - **Descripción/Enfoque**: Detalles adicionales (opcional)
   - **Personaje**: Nombre y género del protagonista
   - **Estilo Visual**: Selecciona el estilo artístico
   - **Géneros**: Elige el tono narrativo
   - **Ambientación**: Escenario de la historia
   - **Diapositivas**: De 4 a 16 slides

3. **Genera el Guion**:
   - Click en "Generar Guion"
   - Edita manualmente si lo deseas
   - Aprove el guion antes de generar imágenes

4. **Genera las Imágenes**:
   - Selecciona el modelo de imagen preferido
   - Click en "Generar Diapositivas"
   - Cada slide puede regenerarse individualmente si no te gusta

5. **Gestiona y Descarga**:
   - Elimina slides que no desees incluir
   - Descarga en ZIP, HTML o Tira Cómica

## 📦 Estructura del Proyecto

```
132_Combinacion_Perfecta-V1/
├── index.html          # Aplicación principal (HTML + CSS + JS)
├── README.md           # Este archivo
└── 127_Generador_de_comics-V2/  # Referencia de implementación por lotes
    └── script.js
```

## 🛠️ Tecnologías

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **API de Texto**: Pollinations AI (`gen.pollinations.ai/v1/chat/completions`)
- **API de Imagen**: Pollinations AI (`enter.pollinations.ai/api/generate/image`)
- **Compresión**: JSZip para descargas ZIP
- **Estilos**: Diseño dark mode responsive

## 🎨 Estilos Visuales Disponibles

| Categoría | Estilos |
|-----------|---------|
| **3D/CGI** | Pixar, Disney, Cartoon 3D, Minions |
| **Anime** | Anime/Manga, Studio Ghibli, Chibi, Shonen, Shojo |
| **Cómic** | Marvel/DC, Línea Clara (Tintín), Webtoon, Europeo |
| **Retro** | Pop Art, Hanna-Barbera, Looney Tunes, 80s Comic |
| **Artístico** | Acuarela, Boceto a Lápiz, Pixel Art, Noir |
| **Especial** | Cyberpunk, Steampunk, South Park, Cuentos de Hadas |

## 🌟 Características Avanzadas

### Generación por Lotes
Para guiones de 11+ diapositivas, la aplicación automáticamente:
- Divide la generación en lotes de 6 slides
- Preserva la continuidad narrativa entre lotes
- Concatena todos los lotes en un guion final coherente

### Tira Cómica HTML
El formato de descarga "Tira Cómica" genera:
- Página HTML con grid de 2 columnas (responsive a 1 en móvil)
- Header con el tema de la historieta como título
- Cada panel clickeable abre modal con imagen ampliada
- Cierre del modal al hacer clic o presionar ESC
- Imágenes embebidas en base64 (archivo portable)

### Gestión de Diapositivas
- Cada slide tiene botón 🗑️ Eliminar / ↩️ Restaurar
- Slides eliminadas se marcan visualmente (grayscale + badge)
- Las eliminadas se excluyen de todas las descargas
- Permite curar el contenido final antes de exportar

## 📱 Compatibilidad

- Chrome/Edge/Firefox/Safari (últimas versiones)
- Diseño responsive para tablets
- No requiere instalación ni backend

## 🔒 Privacidad

- La API Key se almacena localmente en tu navegador (`localStorage`)
- Ningún dato se envía a servidores propios
- Todo el procesamiento ocurre en tu dispositivo

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Libre para uso personal y educativo.

---

**Diseñado por Juan Guillermo Rivera Berrío** con tecnología Gemini 3 Pro

⭐ ¡Si te gusta este proyecto, dale una estrella en GitHub!
