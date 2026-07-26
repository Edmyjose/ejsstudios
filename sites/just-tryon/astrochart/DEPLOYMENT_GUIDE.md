# GUÍA DE DESPLIEGUE - SUBDOMINIO astrochart.ejsstudios.com

## 📋 INFORMACIÓN DEL PROYECTO

**Sitio principal:** `https://ejsstudios.com/`  
**Subdominio:** `https://astrochart.ejsstudios.com/`  
**App:** Birth Chart Generator (Android)  
**ID de App:** `com.ejs.birthchart`  
**Google Play:** `https://play.google.com/store/apps/details?id=com.ejs.birthchart`

## 🗂️ ESTRUCTURA DE ARCHIVOS PARA EL SUBDOMINIO

### **OPCIÓN 1: Carpeta raíz del subdominio**
```
/ (directorio raíz de astrochart.ejsstudios.com)
├── index.html                    # Landing page principal
├── images/                       # Carpeta para imágenes
│   ├── screenshot1.png           # 1080x1920px
│   ├── screenshot2.png           # 1080x1920px  
│   ├── screenshot3.png           # 1080x1920px
│   ├── screenshot4.png           # 1080x1920px
│   ├── og-image.jpg              # 1200x630px
│   ├── twitter-card.jpg          # 1200x600px
│   └── favicon.ico               # Favicon
├── .htaccess                     # Configuración Apache (opcional)
└── robots.txt                    # Configuración robots (opcional)
```

### **OPCIÓN 2: Subcarpeta en sitio principal**
```
/ (directorio raíz de ejsstudios.com)
├── astrochart/                   # Subcarpeta del subdominio
│   ├── index.html                # Landing page principal
│   └── images/                   # Carpeta para imágenes
└── (resto del sitio principal)
```

## 🔧 CONFIGURACIÓN DEL SUBDOMINIO

### **1. Crear el subdominio en cPanel/Hosting:**
```
1. Acceder a cPanel de ejsstudios.com
2. Ir a "Subdominios"
3. Crear nuevo subdominio:
   - Nombre: astrochart
   - Directorio: public_html/astrochart
   - Crear directorio automáticamente: ✅
```

### **2. Configurar DNS (si no es automático):**
```
Registro DNS:
- Tipo: A
- Nombre: astrochart
- Valor/Dirección: IP del servidor de ejsstudios.com
- TTL: 14400 (4 horas)
```

### **3. Cargar archivos via FTP:**
```
1. Conectarse a FTP de ejsstudios.com
2. Navegar a: /public_html/astrochart/
3. Subir archivos:
   - index.html
   - Carpeta /images/ con todas las imágenes
```

## 🖼️ GENERAR IMÁGENES NECESARIAS

### **Imágenes obligatorias:**
1. **Screenshots** (1080x1920px cada una):
   - `screenshot1.png` - Pantalla principal de carta natal
   - `screenshot2.png` - Interpretación con IA
   - `screenshot3.png` - Horóscopo diario
   - `screenshot4.png` - Calculadora de numerología

2. **Imágenes sociales:**
   - `og-image.jpg` (1200x630px) - Para Facebook/Open Graph
   - `twitter-card.jpg` (1200x600px) - Para Twitter

3. **Favicons:**
   - `favicon.ico` (16x16, 32x32, 48x48)
   - `favicon-16x16.png`, `favicon-32x32.png`
   - `apple-touch-icon.png` (180x180)

### **Prompts actualizados para tu dominio:**

**OG Image (1200x630):**
```
"Professional astrology app banner showing 'Birth Chart Generator by EJS Studios' 
with zodiac wheel and AI brain icon. Purple/blue gradient background with stars. 
Include text: 'Available on Google Play - astrochart.ejsstudios.com'. Clean, 
modern design suitable for social media sharing."
```

**Twitter Card (1200x600):**
```
"Twitter card for Birth Chart Generator app by EJS Studios. Show app icon, 
zodiac wheel, and text 'Scientific Astrology with AI'. Include hashtags 
#astrology #AI #androidapp and website astrochart.ejsstudios.com"
```

## 🔍 SEO Y META TAGS VERIFICADOS

### **URLs configuradas en index.html:**
- ✅ `og:url`: `https://astrochart.ejsstudios.com/`
- ✅ `twitter:url`: `https://astrochart.ejsstudios.com/`
- ✅ `canonical`: `https://astrochart.ejsstudios.com/`
- ✅ `og:image`: `https://astrochart.ejsstudios.com/images/og-image.jpg`
- ✅ `twitter:image`: `https://astrochart.ejsstudios.com/images/twitter-card.jpg`

### **Schema.org actualizado:**
- ✅ Author URL: `https://ejsstudios.com/`
- ✅ Screenshot URLs: `https://astrochart.ejsstudios.com/images/screenshotX.png`
- ✅ Organization URL: `https://ejsstudios.com`

## 🚀 PASOS DE DESPLIEGUE

### **Paso 1: Generar imágenes**
```bash
1. Usar Leonardo.ai o Midjourney con los prompts anteriores
2. Ajustar tamaños exactos:
   - Screenshots: 1080x1920px
   - OG Image: 1200x630px
   - Twitter Card: 1200x600px
3. Comprimir con TinyPNG.com (<200KB cada una)
```

### **Paso 2: Preparar estructura de carpetas**
```bash
1. Crear carpeta local: astrochart/
2. Dentro, crear subcarpeta: images/
3. Copiar index.html a la raíz
4. Copiar todas las imágenes a images/
```

### **Paso 3: Subir al servidor**
```bash
Via FTP (ejemplo con FileZilla):
1. Host: ftp.ejsstudios.com
2. Usuario: tu_usuario
3. Password: tu_password
4. Puerto: 21 (o el que uses)
5. Navegar a: /public_html/astrochart/
6. Subir TODOS los archivos
```

### **Paso 4: Configurar redirecciones (opcional)**
Crear archivo `.htaccess` en la raíz:
```apache
# Redireccionar www a non-www
RewriteEngine On
RewriteCond %{HTTP_HOST} ^www\.astrochart\.ejsstudios\.com [NC]
RewriteRule ^(.*)$ https://astrochart.ejsstudios.com/$1 [L,R=301]

# Redireccionar HTTP a HTTPS
RewriteCond %{HTTPS} off
RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]

# Cache para imágenes
<FilesMatch "\.(jpg|jpeg|png|gif|ico)$">
    Header set Cache-Control "max-age=2592000, public"
</FilesMatch>
```

### **Paso 5: Crear robots.txt**
Crear archivo `robots.txt`:
```txt
User-agent: *
Allow: /
Disallow: /admin/
Disallow: /private/

Sitemap: https://astrochart.ejsstudios.com/sitemap.xml
```

## ✅ VERIFICACIÓN POST-DESPLIEGUE

### **Herramientas de verificación:**
1. **URL Directa:** `https://astrochart.ejsstudios.com/`
2. **Facebook Debugger:** `https://developers.facebook.com/tools/debug/`
3. **Twitter Card Validator:** `https://cards-dev.twitter.com/validator`
4. **Google PageSpeed Insights:** `https://pagespeed.web.dev/`
5. **Mobile-Friendly Test:** `https://search.google.com/test/mobile-friendly`

### **Checklist de verificación:**
- [ ] Página carga correctamente
- [ ] Todas las imágenes se muestran
- [ ] Botones de Google Play funcionan
- [ ] Cambio de idioma funciona
- [ ] Meta tags aparecen en redes sociales
- [ ] Mobile responsive funciona
- [ ] SSL/HTTPS activado (certificado)
- [ ] Caché de imágenes configurado

## 🔗 INTEGRACIÓN CON SITIO PRINCIPAL

### **Enlaces desde ejsstudios.com:**
Agregar en tu sitio principal:
```html
<!-- En el footer o menú de ejsstudios.com -->
<a href="https://astrochart.ejsstudios.com/" target="_blank">
    <i class="fas fa-star"></i> Birth Chart Generator App
</a>
```

### **Google Search Console:**
1. Agregar propiedad: `https://astrochart.ejsstudios.com/`
2. Verificar propiedad (archivo HTML o DNS)
3. Enviar sitemap (opcional)
4. Monitorear indexación

### **Google Analytics:**
1. Crear nueva propiedad para el subdominio
2. Obtener GA4 Measurement ID: `G-XXXXXXXXXX`
3. Reemplazar en línea 579 del index.html
4. Verificar que tracking funciona

## ⚠️ SOLUCIÓN DE PROBLEMAS COMUNES

### **Imágenes no cargan:**
```bash
1. Verificar permisos de carpeta /images/ (755)
2. Verificar que rutas sean correctas:
   - index.html usa: src="images/nombre.png"
   - Las imágenes deben estar en /images/
3. Probar URL directa: https://astrochart.ejsstudios.com/images/screenshot1.png
```

### **Subdominio no resuelve:**
```bash
1. Verificar DNS propagation (puede tomar 24-48 horas)
2. Verificar configuración en cPanel
3. Probar con: ping astrochart.ejsstudios.com
4. Esperar 1 hora y limpiar caché DNS local
```

### **SSL/HTTPS issues:**
```bash
1. En cPanel, usar Let's Encrypt SSL
2. Aplicar certificado SSL a subdominio
3. Forzar HTTPS en .htaccess
4. Probar con: https://www.sslshopper.com/ssl-checker.html
```

## 📊 ANÁLISIS Y MONITOREO

### **Métricas a monitorear:**
1. **Tráfico:** Visitas únicas, páginas vistas
2. **Conversiones:** Clicks a Google Play Store
3. **Comportamiento:** Tiempo en página, bounce rate
4. **Dispositivos:** Mobile vs Desktop
5. **Fuentes:** Búsqueda directa, redes sociales, referidos

### **Mejoras futuras:**
1. Añadir formulario de contacto
2. Integrar newsletter opt-in
3. Añadir blog/posts sobre astrología
4. Crear página de Privacy Policy/Terms
5. Añadir más testimonios cuando tengas usuarios

## 🎯 RECOMENDACIONES FINALES

### **Para SEO local:**
1. Agregar dirección física si tienes oficina
2. Incluir schema.org LocalBusiness
3. Crear Google My Business para la app
4. Solicitar reseñas en Google Play

### **Para marketing:**
1. Compartir en redes sociales con hashtags
2. Crear anuncios Google Ads para la app
3. Hacer outreach a blogs de astrología
4. Participar en foros relevantes

### **Para analítica:**
1. Configurar goals en Google Analytics
2. Monitorear eventos específicos
3. Hacer A/B testing de CTAs
4. Analizar funnel de conversión

---

## ⏱️ TIMELINE ESTIMADO

**Total: 2-4 horas de trabajo**

1. **Generar imágenes:** 1-2 horas
2. **Configurar subdominio:** 15-30 minutos
3. **Subir archivos:** 15-30 minutos
4. **Verificación y testing:** 30-60 minutos
5. **Configurar analytics:** 15-30 minutos

---

**¡Tu landing page estará lista en `https://astrochart.ejsstudios.com/` y completamente integrada con tu sitio principal `https://ejsstudios.com/`!**
