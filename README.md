# KIP App Website

Sitio web oficial de KIP App (Kid's Interactive Programming) - Una herramienta educativa para el aprendizaje de programación básica diseñada especialmente para estudiantes del sector rural.

## 🚀 Características

- **Diseño Responsive**: Optimizado para dispositivos móviles y escritorio
- **Descargas Reales**: Sistema de descarga funcional para múltiples plataformas
- **Manual Interactivo**: Guía completa de usuario con navegación por pestañas
- **Animaciones Suaves**: Efectos visuales y transiciones elegantes
- **Tema Espacial**: Diseño inspirado en el espacio con elementos animados

## 📁 Estructura del Proyecto

\`\`\`
kip-app-website/
├── index.html          # Página principal
├── styles.css          # Estilos CSS
├── script.js           # Funcionalidad JavaScript
├── downloads/          # Carpeta para archivos descargables
│   ├── KIP-App-Windows-v1.0.0.exe
│   ├── KIP-App-macOS-v1.0.0.dmg
│   ├── KIP-App-Linux-v1.0.0.AppImage
│   ├── KIP-App-Android-v1.0.0.apk
│   └── KIP-App-Manual-v1.0.0.pdf
├── images/             # Imágenes del sitio
│   ├── kip-login.png
│   ├── kip-game.png
│   └── kip-profile.png
└── README.md           # Este archivo
\`\`\`

## 🔧 Configuración de Descargas

### Paso 1: Crear la carpeta de descargas

\`\`\`bash
mkdir downloads
\`\`\`

### Paso 2: Agregar tus archivos

Coloca tus archivos ejecutables en la carpeta `downloads/` con los siguientes nombres:

- **Windows**: `KIP-App-Windows-v1.0.0.exe`
- **macOS**: `KIP-App-macOS-v1.0.0.dmg`
- **Linux**: `KIP-App-Linux-v1.0.0.AppImage`
- **Android**: `KIP-App-Android-v1.0.0.apk`
- **Manual**: `KIP-App-Manual-v1.0.0.pdf`

### Paso 3: Habilitar descargas

En el archivo `script.js`, cambia la función `checkFileExists()`:

\`\`\`javascript
function checkFileExists(url) {
  // Cambiar a true cuando tengas los archivos
  return true  // Cambiar de false a true
}
\`\`\`

## 🌐 Despliegue

### GitHub Pages

1. **Sube el proyecto a GitHub:**
\`\`\`bash
git init
git add .
git commit -m "Initial commit - KIP App Website"
git remote add origin https://github.com/TU-USUARIO/kip-app-website.git
git push -u origin main
\`\`\`

2. **Activa GitHub Pages:**
   - Ve a Settings → Pages
   - Selecciona "Deploy from a branch"
   - Elige "main" branch
   - Tu sitio estará en: `https://TU-USUARIO.github.io/kip-app-website`

### Netlify

1. Arrastra la carpeta del proyecto a [netlify.com/drop](https://netlify.com/drop)
2. O conecta tu repositorio de GitHub para despliegue automático

### Vercel

\`\`\`bash
npm i -g vercel
vercel --prod
\`\`\`

## 📱 Funcionalidades

### Descargas Inteligentes
- Detección automática de plataforma
- Notificaciones de descarga
- Fallback para archivos no disponibles
- Tracking de descargas (opcional)

### Manual Interactivo
- Navegación por pestañas
- Búsqueda por teclado (flechas arriba/abajo)
- Contenido organizado por secciones

### Responsive Design
- Menú móvil funcional
- Grid adaptativo
- Imágenes optimizadas
- Tipografía escalable

## 🎨 Personalización

### Colores
Edita las variables CSS en `styles.css`:

\`\`\`css
:root {
  --primary-blue: #3b82f6;
  --primary-green: #059669;
  --background-dark: #111827;
  --text-light: #d1d5db;
}
\`\`\`

### Archivos de Descarga
Actualiza las URLs en `script.js`:

\`\`\`javascript
const downloadConfig = {
  desktop: {
    windows: {
      url: "downloads/TU-ARCHIVO.exe",
      filename: "TU-ARCHIVO.exe",
      size: "XX.X MB"
    }
    // ... más configuraciones
  }
}
\`\`\`

## 🛠️ Desarrollo Local

1. **Clona el repositorio:**
\`\`\`bash
git clone https://github.com/TU-USUARIO/kip-app-website.git
cd kip-app-website
\`\`\`

2. **Abre con Live Server:**
   - Usa la extensión Live Server de VS Code
   - O cualquier servidor local (Python, Node.js, etc.)

3. **Servidor Python simple:**
\`\`\`bash
python -m http.server 8000
\`\`\`

## 📊 Analytics (Opcional)

Para agregar Google Analytics, añade en `<head>`:

\`\`\`html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
\`\`\`

## 🤝 Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver `LICENSE` para más detalles.

## 👥 Equipo

- Josué David Díaz Flórez
- Andrés Sebastián Mejía Pinzón  
- Angela Paola Orihuela Beltrán
- Alejandro Ascanio Vera
- Diego Andrés Gómez Gallego
- Milton Andrés Guillen

**SENA - Ficha 2825962**  
Centro de Formación para el Desarrollo Rural y Minero  
Cúcuta, Norte de Santander - Colombia

## 📞 Soporte

¿Necesitas ayuda? Contacta al equipo de desarrollo o abre un issue en GitHub.

---

⭐ **¡No olvides dar una estrella al proyecto si te fue útil!**
