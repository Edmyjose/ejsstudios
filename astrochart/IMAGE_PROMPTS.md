# PROMPTS PARA IMÁGENES - LANDING PAGE

## 📱 IMÁGENES PARA CAPTURAS DE PANTALLA (Mobile Screenshots)

### **IMAGEN 1: Main Birth Chart Screen**
**Tamaño:** 1080x1920px (Mobile screenshot ratio)
**Estilo:** Modern Android app screenshot
**Prompt:**
```
"Modern Android app screen showing an interactive birth chart with zodiac wheel, 
planets positions, and clean material design UI. Dark theme with purple accents, 
showing user birth data input fields (date, time, location). Professional, clean 
astrology app interface with Kotlin/Jetpack Compose aesthetic. Include subtle 
gradient background from dark blue to purple. Show zodiac symbols around wheel."
```

### **IMAGEN 2: AI Interpretation Screen**
**Tamaño:** 1080x1920px (Mobile screenshot ratio)
**Estilo:** Chat interface with AI responses
**Prompt:**
```
"Android app screen showing AI-generated astrology interpretation with Gemini AI 
logo visible. Chat interface showing personalized reading about planetary positions 
and aspects. Clean, modern design with gradient purple/blue background. Show 
conversation bubbles with AI insights about sun, moon, and rising signs. Include 
'Generate New Insight' button at bottom."
```

### **IMAGEN 3: Daily Horoscope Screen**
**Tamaño:** 1080x1920px (Mobile screenshot ratio)
**Estilo:** Zodiac signs with daily predictions
**Prompt:**
```
"Mobile app daily horoscope screen showing all 12 zodiac signs in a grid layout 
with today's predictions. Colorful zodiac icons (Aries, Taurus, Gemini, etc.), 
personalized recommendations, clean typography. Modern astrology app design with 
'Your Sign Today' highlighted. Include love, career, and health insights for each 
sign. Soft gradient background."
```

### **IMAGEN 4: Numerology Calculator**
**Tamaño:** 1080x1920px (Mobile screenshot ratio)
**Estilo:** Numerology calculation interface
**Prompt:**
```
"Numerology calculator screen in astrology app showing life path number calculation, 
expression number, soul urge number with detailed explanations. Clean UI with 
large numbers visualization (7, 11, 22, etc.) and mystical aesthetic. Include 
birth date input fields and results visualization. Modern design with purple/blue 
color scheme and subtle geometric patterns."
```

---

## 🎨 IMÁGENES ADICIONALES (Opcionales pero recomendadas)

### **HERO BACKGROUND IMAGE**
**Tamaño:** 1920x1080px (Desktop background)
**Estilo:** Abstract cosmic background
**Prompt:**
```
"Abstract cosmic background with stars, nebula, and subtle zodiac constellations. 
Deep space aesthetic with purple/blue gradient. Suitable for website hero section. 
Ethereal, mystical, but modern and clean. Include subtle geometric patterns 
representing astrology charts."
```

### **APP ICON/FEATURE ICONS**
**Tamaño:** 512x512px (App icon) y 128x128px (feature icons)
**Estilo:** Modern flat/line icons

**App Icon Prompt:**
```
"Modern astrology app icon featuring stylized zodiac wheel with integrated AI 
circuit patterns. Purple and blue gradient, clean lines, professional appearance. 
Suitable for Google Play Store. Combine celestial and technology aesthetics."
```

**Feature Icons (4 needed):**
1. **Calculator Icon:** "Stylized calculator with zodiac symbols integrated"
2. **AI Icon:** "Abstract AI/robot head with constellation patterns"
3. **Chart Icon:** "Interactive chart/graph with planetary symbols"
4. **Moon Icon:** "Crescent moon with stars and mystical elements"

---

## 🛠️ HERRAMIENTAS RECOMENDADAS PARA GENERAR IMÁGENES

### **Gratuitas:**
1. **Leonardo.ai** - 150 créditos gratis al día
2. **Playground AI** - Gratuito con límites
3. **Bing Image Creator** - Gratuito con Microsoft account
4. **Stable Diffusion Online** - Varios sitios gratuitos

### **De Pago (mejor calidad):**
1. **Midjourney** - $10-30/mes (mejor calidad)
2. **DALL-E 3** - Vía ChatGPT Plus
3. **Adobe Firefly** - Integrado en Creative Cloud

### **Para editar/tamañar:**
1. **Canva** - Para ajustar tamaños y agregar texto
2. **Photopea** - Editor online gratis tipo Photoshop
3. **GIMP** - Editor de código abierto

---

## 📁 ESTRUCTURA DE ARCHIVOS RECOMENDADA

```
landing-page/
├── index.html              # Archivo principal
├── style.css              # Estilos (opcional separar)
├── script.js              # JavaScript (opcional separar)
├── images/
│   ├── screenshots/
│   │   ├── screenshot1.png    # 1080x1920
│   │   ├── screenshot2.png    # 1080x1920
│   │   ├── screenshot3.png    # 1080x1920
│   │   └── screenshot4.png    # 1080x1920
│   ├── hero-bg.jpg        # 1920x1080 (opcional)
│   └── icons/
│       ├── app-icon.png   # 512x512
│       ├── calculator-icon.png # 128x128
│       ├── ai-icon.png    # 128x128
│       ├── chart-icon.png # 128x128
│       └── moon-icon.png  # 128x128
└── README.md
```

---

## 🚀 PASOS PARA SUBIR AL SERVIDOR

### **1. Generar las imágenes:**
```bash
Usar los prompts anteriores en:
- Leonardo.ai (gratis) o
- Midjourney/DALL-E (mejor calidad)

Guardar como PNG con fondo transparente si es posible.
```

### **2. Ajustar tamaños:**
```bash
Usar Canva o Photopea para:
- Asegurar que screenshots sean 1080x1920px
- Recortar y ajustar según necesidad
- Optimizar peso (<200KB cada una)
```

### **3. Subir al servidor:**
```bash
1. Crear carpeta 'images' en tu servidor
2. Subir todas las imágenes generadas
3. Ajustar rutas en index.html si es necesario
4. Probar que todas las imágenes carguen
```

### **4. Personalizar la landing page:**
```html
<!-- Cambiar estos enlaces según tu configuración -->
<button class="play-store-btn" onclick="window.open('https://play.google.com/store/apps/details?id=com.ejs.birthchart')">
<!-- Y -->
<button class="download-btn" onclick="window.open('tu-enlace-de-descarga.apk')">
```

---

## 💡 TIPS PARA GENERAR MEJORES IMÁGENES

### **En Leonardo.ai/Midjourney:**
```
1. Usar --ar 9:16 para mobile screenshots (1080x1920)
2. Agregar "clean UI", "material design", "modern app" en prompts
3. Especificar "dark theme with purple accents"
4. Pedir "no text" o "minimal text" para más versatilidad
5. Generar varias variaciones y elegir la mejor
```

### **Para consistencia visual:**
```
- Mismo esquema de colores en todas (purple/blue gradient)
- Mismo estilo de interfaz (Material Design)
- Mismas tipografías implícitas (sans-serif, clean)
- Mismo nivel de detalle y realismo
```

### **Si no puedes generar imágenes:**
```html
<!-- Usar placeholders temporales -->
<img src="https://via.placeholder.com/1080x1920/6a11cb/ffffff?text=Birth+Chart+Screen" class="screenshot">
```

---

## 🔗 ENLACES ÚTILES

1. **Leonardo.ai:** https://leonardo.ai
2. **Midjourney:** https://midjourney.com
3. **Canva:** https://canva.com
4. **Photopea:** https://photopea.com
5. **TinyPNG:** https://tinypng.com (para comprimir imágenes)

---

## ✅ CHECKLIST FINAL

### **Antes de subir:**
- [ ] Todas las imágenes generadas y optimizadas
- [ ] Screenshots en tamaño correcto (1080x1920)
- [ ] Imágenes comprimidas (<200KB cada una)
- [ ] Enlaces en botones actualizados
- [ ] Textos revisados (español/inglés)
- [ ] Funcionalidad probada localmente
- [ ] Mobile responsive probado

### **Después de subir:**
- [ ] Todas las imágenes cargan correctamente
- [ ] Botones funcionan (abren enlaces correctos)
- [ ] Cambio de idioma funciona
- [ ] Scroll smooth funciona
- [ ] SEO básico (meta tags podrían agregarse después)
- [ ] Analytics/configurado (opcional)

---

**¡Tu landing page está lista para personalizar y publicar!**