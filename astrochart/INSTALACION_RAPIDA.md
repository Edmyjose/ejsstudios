# 📋 INSTALACIÓN RÁPIDA - astrochart.ejsstudios.com

## 🚀 PASOS EN 10 MINUTOS

### **1. Crear subdominio (cPanel)**
```
1. Login a cPanel de ejsstudios.com
2. Ir a "Subdominios"
3. Crear: astrochart → public_html/astrochart
4. Aplicar SSL Let's Encrypt al subdominio
```

### **2. Subir archivos (FTP)**
```
Carpeta destino: /public_html/astrochart/

ARCHIVOS A SUBIR:
✅ index.html          (archivo principal)
✅ .htaccess           (configuración)
✅ robots.txt          (para SEO)
✅ images/             (carpeta con imágenes)
```

### **3. Generar imágenes mínimas**
**Obligatorias:**
- `images/screenshot1.png` - 1080x1920px (carta natal)
- `images/screenshot2.png` - 1080x1920px (IA)
- `images/screenshot3.png` - 1080x1920px (horóscopo)
- `images/screenshot4.png` - 1080x1920px (numerología)
- `images/favicon.ico` - 16x16, 32x32, 48x48

**Opcionales (pero recomendadas):**
- `images/og-image.jpg` - 1200x630px (Facebook)
- `images/twitter-card.jpg` - 1200x600px (Twitter)

### **4. Verificar funcionamiento**
```
1. Abrir: https://astrochart.ejsstudios.com/
2. Probar botones de Google Play
3. Probar cambio de idioma
4. Verificar en mobile
```

## 🔧 CONFIGURACIÓN PERSONALIZADA

### **En index.html (BUSCAR Y REEMPLAZAR):**
1. **Google Analytics** (línea ~579):
   ```javascript
   gtag('config', 'G-XXXXXXXXXX'); // REEMPLAZAR CON TU ID
   ```

2. **Email de contacto** (línea ~1051):
   ```html
   <li><i class="fas fa-envelope"></i>info@ejsstudios.com</li>
   ```

## ✅ CHECKLIST FINAL

### **Antes de publicar:**
- [ ] Subdominio creado: astrochart.ejsstudios.com
- [ ] SSL instalado (candado verde)
- [ ] Archivos subidos a /public_html/astrochart/
- [ ] Imágenes generadas en carpeta /images/
- [ ] Google Analytics configurado

### **Después de publicar:**
- [ ] URL funciona: https://astrochart.ejsstudios.com/
- [ ] Todas las imágenes cargan
- [ ] Botones de Play Store funcionan
- [ ] Cambio de idioma funciona
- [ ] Mobile responsive OK
- [ ] SSL/HTTPS activado

## 🆘 SOLUCIÓN RÁPIDA DE PROBLEMAS

### **Si no carga:**
```
1. Esperar 30 min (propagación DNS)
2. Verificar subdominio en cPanel
3. Probar sin cache: Ctrl+F5
```

### **Si imágenes no aparecen:**
```
1. Verificar carpeta /images/ existe
2. Verificar nombres de archivo exactos
3. Probar URL directa: astrochart.ejsstudios.com/images/screenshot1.png
```

### **Si SSL no funciona:**
```
1. En cPanel: Let's Encrypt SSL
2. Aplicar al subdominio astrochart
3. Esperar 5 min y recargar
```

## 📞 CONTACTO RÁPIDO

**Archivos modificados:**
- ✅ index.html - Landing page completa
- ✅ .htaccess - Configuración servidor
- ✅ robots.txt - Configuración SEO
- ✅ INSTALACION_RAPIDA.md - Estas instrucciones

**URL final:** `https://astrochart.ejsstudios.com/`

**Tiempo estimado:** 10-30 minutos

**¡Listo para lanzar! 🚀**
