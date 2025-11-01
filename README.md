# AgendaNova - Landing Page

Landing page estática para **AgendaNova**, sistema de gestión de citas para profesionales de salud.

## 🚀 Descripción

Este sitio web es una página de presentación (landing page) completamente estática diseñada para mostrar el sistema AgendaNova. Incluye:

- Sección hero con llamados a la acción
- Video demo incrustado de YouTube
- Lista de beneficios y funcionalidades
- Proceso de trabajo en 3 pasos
- Sección "Quién soy"
- Formularios de contacto (WhatsApp y email)

## 📁 Estructura del proyecto
```
/
├── index.html          # Página principal
├── styles.css          # Estilos CSS
├── README.md           # Este archivo
└── assets/
    ├── logo.png        # Logo de AgendaNova (reemplazar)
    └── thumbnail.jpg   # Imagen para Open Graph (opcional)
```

## ✏️ Personalización

Antes de publicar, debes reemplazar los siguientes elementos:

### 1. **Número de WhatsApp**
Busca en `index.html` todas las instancias de:
```html
https://wa.me/51XXXXXXXX
```
Y reemplázalas con tu número real (sin espacios ni signos). Ejemplo:
```html
https://wa.me/51987654321
```

### 2. **Email de contacto**
Busca en `index.html`:
```html
mailto:tu@correo.com
```
Y reemplázalo con tu email real. Ejemplo:
```html
mailto:sebastian@agendanova.com
```

### 3. **Número en el footer**
Busca en el `<footer>`:
```html
Contacto: +51 XXXXXXXX
```
Y reemplázalo con tu número de contacto visible.

### 4. **Logo e imágenes**
- Reemplaza `assets/logo.png` con tu logo real (recomendado: 180x40px o proporcional)
- Opcionalmente, agrega `assets/thumbnail.jpg` (1200x630px) para Open Graph

### 5. **Video de YouTube**
Si deseas cambiar el video demo, busca en `index.html`:
```html
src="https://www.youtube.com/embed/WQDbBJIk6Oc"
```
Y reemplaza el ID del video (`WQDbBJIk6Oc`) con el tuyo.

## 🌐 Desplegar en GitHub Pages

### Paso 1: Crear repositorio en GitHub
1. Ve a [GitHub](https://github.com) e inicia sesión
2. Haz clic en el botón **"New"** (o "+") para crear un nuevo repositorio
3. Nómbralo como prefieras (ej: `agendanova-landing`)
4. Marca como **público**
5. **No** inicialices con README (ya tienes uno)
6. Haz clic en **"Create repository"**

### Paso 2: Subir archivos desde tu computadora

Abre tu terminal en la carpeta del proyecto y ejecuta:
```bash
git init
git add .
git commit -m "Primera versión de AgendaNova landing"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/TU_REPO.git
git push -u origin main
```

> **Nota:** Reemplaza `TU_USUARIO` y `TU_REPO` con tus datos reales de GitHub.

### Paso 3: Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **"Settings"** (Configuración)
3. En el menú lateral izquierdo, busca **"Pages"**
4. En **"Source"**, selecciona:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
5. Haz clic en **"Save"**
6. Espera 1-2 minutos y recarga la página
7. Verás un mensaje: **"Your site is live at https://TU_USUARIO.github.io/TU_REPO/"**

¡Listo! Tu landing page está publicada.

## 🔄 Actualizar el sitio

Cada vez que hagas cambios:
```bash
git add .
git commit -m "Descripción del cambio"
git push
```

GitHub Pages se actualizará automáticamente en 1-2 minutos.

## 📱 Probar en local

Puedes abrir directamente `index.html` en tu navegador, o usar un servidor local:
```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (si tienes npx)
npx serve
```

Luego abre `http://localhost:8000` en tu navegador.

## 🎨 Modificar colores

Los colores principales están definidos como variables CSS en `styles.css`:
```css
:root {
    --color-primary: #2563eb;        /* Azul principal */
    --color-primary-dark: #1e40af;   /* Azul oscuro (hover) */
    --color-secondary: #64748b;      /* Gris secundario */
    --color-text: #1e293b;           /* Texto principal */
    --color-text-light: #64748b;     /* Texto secundario */
}
```

Modifica estos valores para cambiar la paleta de colores.

## 📄 Licencia

Este proyecto es de uso personal para Sebastián Morales / AgendaNova.

## 💬 Soporte

Para dudas sobre el código, contacta al desarrollador que te entregó estos archivos.