# Propuesta web — Consultorio Odontológico Kennedy

Rediseño moderno y **responsive** (funciona en celular) de la web de la clínica,
hecho como propuesta para mostrar por WhatsApp y cobrar la mejora.

## Qué incluye / qué mejora vs la web actual
- ✅ **100% responsive** (la web actual no se ve bien en celular — su problema #1)
- ✅ Diseño moderno con su branding real ("Luce una mejor sonrisa", Dr. Javier Blanco)
- ✅ **Botón de WhatsApp flotante** + CTAs que abren el chat con mensaje pre-cargado
- ✅ Sus servicios reales en tarjetas, sección "nosotros", galería con sus fotos
- ✅ Mapa de Google con su dirección real
- ✅ SEO básico (title + meta description, que la web actual no tenía bien)
- ✅ Carga rápida (un solo archivo + imágenes optimizadas)

## ⚠️ Nota sobre las reseñas
La calificación **4.8 ⭐ y "98 opiniones"** son REALES (de su Google) y el botón lleva
a su perfil real. Las **3 tarjetas de reseña con texto** (María G., Andrés R., Laura M.)
son **ejemplos de muestra** — antes de publicar, reemplazalas por reseñas reales de su
Google (copiá 3 textos reales y sus nombres). Buscá `<!-- REVIEWS` / `id="resenas"` en cada archivo.

## Ver en local
Abrí `index.html` en el navegador (doble clic), o serví la carpeta:
```bash
python -m http.server 8080
# luego abrí http://localhost:8080
```

## Subir a Vercel (para mandar el link por WhatsApp)

**Opción A — Drag & drop (la más fácil, sin instalar nada):**
1. Entrá a https://vercel.com/new
2. Arrastrá esta carpeta completa (`clinica-kennedy-propuesta`)
3. Deploy → te da un link tipo `https://clinica-kennedy-xxxx.vercel.app`

**Opción B — Vercel CLI:**
```bash
npm i -g vercel
cd clinica-kennedy-propuesta
vercel        # seguí los pasos; al terminar te da la URL pública
```

## Cómo enviarlo al cliente (WhatsApp)
Mensaje sugerido a (+57) 311 618 5086:

> Hola Dr. Javier 👋 Vi la web del Consultorio Odontológico Kennedy y noté que
> **no se ve bien en celulares** (donde está el 70% de sus pacientes). Le preparé
> **sin costo** una versión nueva, moderna y que sí funciona en móvil. Échele un
> vistazo: [LINK DE VERCEL]
> Si le gusta, se la dejo lista y optimizada. ¿Le interesa?

## Estructura — 3 propuestas de diseño
```
clinica-kennedy-propuesta/
├── index.html      # SELECTOR: muestra las 3 opciones (es lo que ve el cliente al abrir el link)
├── opcion1.html    # Diseño 1 — Moderno Fresco (turquesa/azul)
├── opcion2.html    # Diseño 2 — Premium Elegante (azul noche + dorado, serif)
├── opcion3.html    # Diseño 3 — Minimal Médico (celeste, formas redondeadas)
└── images/         # fotos reales de la clínica
    ├── clinica1.jpg
    ├── clinica2.jpg
    └── foto4.png
```
Al subir la carpeta a Vercel, el link abre el **selector** con las 3 opciones; el cliente
hace clic en cada una para verla completa. Todas son responsive y con WhatsApp integrado.
