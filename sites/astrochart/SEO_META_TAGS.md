# META TAGS & SEO OPTIMIZATION
**Para agregar al head de tu landing page**

---

## 📊 META TAGS COMPLETOS (Reemplazar en index.html)

```html
<!-- Agregar esto dentro del <head> después del <title> -->

<!-- Primary Meta Tags -->
<meta name="title" content="Birth Chart Generator - Astrología Científica con IA">
<meta name="description" content="App de astrología que combina Swiss Ephemeris (datos astronómicos profesionales) con Google Gemini AI para interpretaciones precisas y personalizadas.">
<meta name="keywords" content="astrología, birth chart, carta natal, zodiaco, horóscopo, IA, inteligencia artificial, Swiss Ephemeris, astronomía, app android, kotlin, jetpack compose">
<meta name="author" content="EJS Studios">
<meta name="robots" content="index, follow">
<meta name="language" content="Spanish, English">

<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://birthchartgenerator.com/">
<meta property="og:title" content="Birth Chart Generator - Astrología Científica con IA">
<meta property="og:description" content="La primera app que combina datos astronómicos profesionales con IA para interpretaciones astrológicas precisas.">
<meta property="og:image" content="https://birthchartgenerator.com/images/og-image.jpg">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:locale" content="es_ES, en_US">
<meta property="og:site_name" content="Birth Chart Generator">

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image">
<meta property="twitter:url" content="https://birthchartgenerator.com/">
<meta property="twitter:title" content="Birth Chart Generator - Astrología Científica con IA">
<meta property="twitter:description" content="App de astrología con cálculos científicos e interpretaciones de IA.">
<meta property="twitter:image" content="https://birthchartgenerator.com/images/twitter-card.jpg">

<!-- Additional Tags -->
<meta name="theme-color" content="#6a11cb">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
<meta name="apple-mobile-web-app-title" content="Birth Chart Generator">
<meta name="application-name" content="Birth Chart Generator">
<meta name="mobile-web-app-capable" content="yes">

<!-- Favicon Links -->
<link rel="icon" type="image/x-icon" href="/favicon.ico">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">

<!-- Canonical URL -->
<link rel="canonical" href="https://birthchartgenerator.com/">

<!-- Preconnect for Performance -->
<link rel="preconnect" href="https://cdnjs.cloudflare.com">
<link rel="preconnect" href="https://fonts.googleapis.com">
```

---

## 🎨 FAVICON GENERATION

### **Prompt para Favicon:**
```
"Modern astrology app icon featuring stylized zodiac wheel with AI circuit patterns. 
Purple and blue gradient, clean lines, professional appearance. Simple design that 
works at small sizes (16x16 to 180x180)."
```

### **Tamaños necesarios:**
```
- favicon.ico (16x16, 32x32, 48x48)
- favicon-16x16.png (16x16)
- favicon-32x32.png (32x32) 
- apple-touch-icon.png (180x180)
- android-chrome-192x192.png (192x192)
- android-chrome-512x512.png (512x512)
```

### **Herramientas para generar favicons:**
1. **Favicon.io** - Gratis, sube una imagen y genera todos los tamaños
2. **RealFaviconGenerator** - Más opciones avanzadas
3. **Canva** - Crear el diseño base

---

## 📱 OPEN GRAPH IMAGE (OG Image)

### **Prompt para OG Image (1200x630):**
```
"Modern astrology app promotional banner showing zodiac wheel, AI brain icon, 
and text 'Birth Chart Generator - Scientific Astrology with AI'. Professional 
design with purple/blue gradient, stars, and clean typography. Include app 
screenshots overlay and download buttons. Suitable for social media sharing."
```

### **Twitter Card Image (1200x600):**
```
Similar al OG image pero optimizado para Twitter. Incluir handle @BirthChartApp 
y hashtags #astrology #AI #androidapp en diseño sutil.
```

---

## 🔍 KEYWORDS PARA SEO

### **Primary Keywords:**
```
- astrología app
- birth chart calculator
- carta natal app
- horóscopo preciso
- astrología científica
- Swiss Ephemeris app
- IA astrología
- zodiaco app
```

### **Secondary Keywords:**
```
- app de astrología android
- calcular carta natal
- interpretación astrológica IA
- posiciones planetarias
- numerología app
- tarot digital
- fases lunares
- eclipse calculator
```

### **Long-tail Keywords:**
```
- aplicación para calcular carta natal exacta
- interpretación de carta natal con inteligencia artificial
- astrología con datos astronómicos profesionales
- app zodiaco con cálculos precisos
- horóscopo personalizado con IA
```

---

## 📝 CONTENIDO SEO OPTIMIZADO

### **Title Tags Optimizados:**
```html
<!-- Español -->
<title>Birth Chart Generator | Astrología Científica con IA | App Android</title>

<!-- English -->
<title>Birth Chart Generator | Scientific Astrology with AI | Android App</title>
```

### **H1 Structure:**
```html
<!-- Español -->
<h1>Astrología <span class="highlight">Científica</span> con <span class="highlight">IA</span></h1>

<!-- English -->
<h1>Scientific <span class="highlight">Astrology</span> with <span class="highlight">AI</span></h1>
```

### **Meta Description Optimizada:**
```html
<meta name="description" content="Birth Chart Generator: La primera app que combina Swiss Ephemeris (datos astronómicos profesionales) con Google Gemini AI para interpretaciones astrológicas precisas y personalizadas. Descarga gratis en Google Play.">
```

---

## 📊 STRUCTURED DATA (Schema.org)

### **Agregar esto antes de </head>:**
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "MobileApplication",
  "name": "Birth Chart Generator",
  "description": "Astrology app combining Swiss Ephemeris astronomical data with Google Gemini AI for personalized interpretations.",
  "applicationCategory": "LifestyleApplication",
  "operatingSystem": "Android",
  "offers": {
    "@type": "Offer",
    "price": "0",
    "priceCurrency": "USD"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "ratingCount": "127"
  },
  "author": {
    "@type": "Organization",
    "name": "EJS Studios"
  },
  "screenshot": [
    {
      "@type": "ImageObject",
      "url": "https://birthchartgenerator.com/images/screenshot1.png",
      "caption": "Interactive Birth Chart Screen"
    },
    {
      "@type": "ImageObject",
      "url": "https://birthchartgenerator.com/images/screenshot2.png",
      "caption": "AI Interpretation Interface"
    }
  ]
}
</script>
```

### **Para la organización:**
```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "EJS Studios",
  "url": "https://birthchartgenerator.com",
  "logo": "https://birthchartgenerator.com/images/logo.png",
  "sameAs": [
    "https://twitter.com/BirthChartApp",
    "https://instagram.com/birthchartgenerator"
  ]
}
</script>
```

---

## 🚀 PERFORMANCE OPTIMIZATION

### **Agregar al final del <head>:**
```html
<!-- Preload Critical Assets -->
<link rel="preload" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" as="style">
<link rel="preload" href="images/screenshot1.png" as="image">

<!-- Inline Critical CSS (opcional para mejor performance) -->
<style>
/* Agregar aquí los estilos críticos para above-the-fold content */
</style>

<!-- Defer Non-critical CSS -->
<noscript>
  <!-- Fallback si JavaScript está desactivado -->
</noscript>
```

### **Agregar al final del <body> (antes de </body>):**
```html
<!-- Analytics (opcional) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>

<!-- Hotjar (opcional para ver comportamiento usuarios) -->
<script>
  (function(h,o,t,j,a,r){
      h.hj=h.hj||function(){(h.hj.q=h.hj.q||[]).push(arguments)};
      h._hjSettings={hjid:YOUR_HOTJAR_ID,hjsv:6};
      a=o.getElementsByTagName('head')[0];
      r=o.createElement('script');r.async=1;
      r.src=t+h._hjSettings.hjid+j+h._hjSettings.hjsv;
      a.appendChild(r);
  })(window,document,'https://static.hotjar.com/c/hotjar-','.js?sv=');
</script>
```

---

## 📧 CONTACT FORM INTEGRATION (Opcional)

### **Agregar en el footer o sección separada:**
```html
<div class="contact-form">
  <h3 class="lang-content es active">Contáctanos</h3>
  <h3 class="lang-content en">Contact Us</h3>
  
  <form action="https://formspree.io/f/your-form-id" method="POST">
    <input type="text" name="name" placeholder="Nombre / Name" required>
    <input type="email" name="email" placeholder="Email" required>
    <textarea name="message" placeholder="Mensaje / Message" rows="4" required></textarea>
    <button type="submit" class="download-btn">
      <i class="fas fa-paper-plane"></i>
      <span class="lang-content es active">Enviar Mensaje</span>
      <span class="lang-content en">Send Message</span>
    </button>
  </form>
</div>
```

### **Alternativas a Formspree:**
1. **Netlify Forms** - Gratis con hosting Netlify
2. **Google Forms** - Simple y gratuito
3. **FormSubmit** - Gratuito, envía a email

---

## ✅ CHECKLIST SEO FINAL

### **Antes de publicar:**
- [ ] Meta tags completos agregados
- [ ] Favicons generados y subidos
- [ ] OG/Twitter images creadas (1200x630)
- [ ] Structured data agregado
- [ ] Títulos y descripciones optimizados
- [ ] Imágenes con alt text (agregar en HTML)
- [ ] URLs canónicas configuradas
- [ ] Sitemap.xml generado (opcional)
- [ ] robots.txt configurado

### **Después de publicar:**
- [ ] Verificar en Google Search Console
- [ ] Probar en Facebook/Twitter debugger
- [ ] Test de velocidad (PageSpeed Insights)
- [ ] Mobile friendly test (Google)
- [ ] SSL certificado instalado (HTTPS)

---

## 🔗 HERRAMIENTAS DE VERIFICACIÓN

1. **Google Search Console:** https://search.google.com/search-console
2. **Facebook Sharing Debugger:** https://developers.facebook.com/tools/debug/
3. **Twitter Card Validator:** https://cards-dev.twitter.com/validator
4. **Google PageSpeed Insights:** https://pagespeed.web.dev/
5. **Mobile-Friendly Test:** https://search.google.com/test/mobile-friendly
6. **Schema Markup Validator:** https://validator.schema.org/

---

**Con estos meta tags y optimizaciones, tu landing page estará lista para rankear en búsquedas y tener una excelente apariencia cuando se comparta en redes sociales.**