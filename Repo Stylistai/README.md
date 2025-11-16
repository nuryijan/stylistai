# 🎨 StylistAI

> Asistente de moda con inteligencia artificial que comprende tus emociones. Ayuda a los usuarios a descubrir su estilo auténtico a través de conversaciones inteligentes.

![Estado](https://img.shields.io/badge/Estado-En_Desarrollo-orange)
![Licencia](https://img.shields.io/badge/Licencia-MIT-blue)
![Plataforma](https://img.shields.io/badge/Plataforma-Vercel-black)

---

## 🌟 Resumen

**StylistAI** es un asistente conversacional bilingüe (español-inglés) que combina inteligencia emocional con moda. A diferencia de los motores de recomendación tradicionales, StylistAI pregunta: **"¿Cómo quieres sentirte hoy?"** en lugar de "¿Qué producto buscas?"

### ✨ Características Principales

- 🎤 **Interacción por Voz** (entrada de texto y voz)
- 💭 **Inteligencia Emocional** - Comprende el estado de ánimo y contexto
- 🎨 **Análisis de Color** - Recomienda colores según tu tono de piel
- 👗 **Conciencia Corporal** - Recomendaciones personalizadas según tipo de cuerpo
- 🌍 **Bilingüe** - Soporte completo en español e inglés
- 📱 **Responsive** - Funciona en desktop, tablet y móvil

---

## 🚀 Comenzar Rápido

### Prerrequisitos

- Node.js 18+ instalado
- Clave API de OpenAI ([obtén una aquí](https://platform.openai.com/api-keys))
- Git instalado
- Cuenta de Vercel (gratis)

### Desarrollo Local

1. **Clona el repositorio**
```bash
git clone https://github.com/nuryijan/stylistai.git
cd stylistai
```

2. **Instala dependencias**
```bash
npm install
```

3. **Configura variables de entorno**
```bash
# Crea un archivo .env.local y agrega:
OPENAI_API_KEY=tu-clave-real-de-openai-aqui
```

4. **Ejecuta localmente**
```bash
npm run dev
```

¡Visita `http://localhost:3000` para ver tu app! 🎉

---

## 📁 Estructura del Proyecto

```
stylistai/
├── .gitignore           # Protege archivos sensibles
├── package.json         # Dependencias
├── vercel.json          # Configuración de despliegue
├── README.md            # Este archivo
├── public/
│   └── index.html       # Interfaz principal (HTML + CSS + JS)
└── api/
    └── chat.js          # Endpoint de conversación
```

---

## 🔑 Variables de Entorno

Crea un archivo `.env.local` en el directorio raíz:

```bash
# Requerida
OPENAI_API_KEY=sk-...

# Opcionales (funcionalidades futuras)
ELEVENLABS_API_KEY=...
PINTEREST_API_KEY=...
```

⚠️ **IMPORTANTE:** Nunca subas `.env.local` a GitHub. Ya está en `.gitignore`.

---

## 🌐 Despliegue en Vercel

### Método 1: Via Dashboard de Vercel (Más Fácil)

1. Sube tu código a GitHub:
```bash
git add .
git commit -m "Commit inicial"
git push origin main
```

2. Ve a [vercel.com](https://vercel.com)
3. Haz clic en "Import Project"
4. Selecciona tu repositorio de GitHub
5. Agrega variables de entorno:
   - `OPENAI_API_KEY` = tu clave de OpenAI
6. Haz clic en "Deploy"

Tu app estará en: `https://stylistai.vercel.app` 🎉

### Método 2: Via CLI de Vercel

```bash
npm install -g vercel
vercel login
vercel --prod
```

---

## 💬 Cómo Funciona

### Flujo del Usuario

1. **Usuario describe la ocasión:**
   > "Tengo una entrevista de trabajo mañana y estoy nerviosa"

2. **AI hace preguntas clarificadoras:**
   > "Para recomendar los mejores colores, ¿tu piel es más cálida (dorada) o fría (rosada)?"

3. **AI analiza el contexto:**
   - Ocasión: Entrevista profesional
   - Estado de ánimo: Nerviosa → necesita confianza
   - Piel: Tono cálido
   - Presupuesto: (pregunta si no se menciona)

4. **AI proporciona recomendaciones personalizadas:**
   - Razonamiento de color: "Los tonos tierra armonizarán con tu tono cálido"
   - Sugerencias de estilo: "Blazer estructurado para autoridad, hombros suaves para accesibilidad"
   - Items específicos: "Esto es lo que buscar en Amazon..."

---

## 🛠️ Stack Tecnológico

- **Frontend:** HTML, CSS, JavaScript vanilla
- **Backend:** Vercel Serverless Functions (Node.js)
- **AI:** OpenAI GPT-4
- **Despliegue:** Vercel Edge Network (CDN global)

---

## 👤 Autor

**Nur Yljan Navarro Urbina**
- GitHub: [@nuryijan](https://github.com/nuryijan)

---

## 📧 Soporte

Si tienes preguntas o necesitas ayuda:
- 📝 Abre un issue en [GitHub](https://github.com/nuryijan/stylistai/issues)
- 📧 Contacto: [tu email]

---

**Hecho con 💜 por Nur Yljan Navarro Urbina**

---

## 🔗 Enlaces

- [Demo en Vivo](https://stylistai.vercel.app)
- [Repositorio GitHub](https://github.com/nuryijan/stylistai)

**¡Recuerda agregar tu `OPENAI_API_KEY` en Vercel para que funcione!** 🔑

---

## 🐛 Solución de Problemas

### "Error de configuración de API"
**Problema:** No se encuentra la clave de OpenAI

**Solución:**
1. Verifica que `OPENAI_API_KEY` esté configurada en Vercel
2. Re-despliega la aplicación

### "Módulo no encontrado"
**Problema:** Dependencias no instaladas

**Solución:**
```bash
npm install
```

### "Error CORS en el navegador"
**Problema:** Ruta API no accesible

**Solución:** Verifica que `vercel.json` esté configurado correctamente

**¡Tu StylistAI está listo para usar!** 🚀



