# Navia — Imagery & Iconografía

## Dirección de arte

Navia usa un estilo visual **cálido, limpio y moderno**. Las imágenes y UI mockups son protagonistas — no decoración. El objetivo es mostrar el producto en contexto real, no imágenes de stock genéricas de viaje.

### Principios

- **Producto primero**: los screenshots de la app son el activo visual más poderoso
- **Calidez**: paleta de imagen alineada con el coral/peach de la marca
- **Modernidad sin frialdad**: mockups en dispositivos reales (celular físico), no en marcos genéricos
- **Minimalismo funcional**: los layouts tienen mucho espacio en blanco — las imágenes respiran

---

## Mockups de app

Los mockups muestran la interfaz de Navia en un iPhone o Android con sombra suave:

```css
/* Contenedor de mockup */
border-radius: 24px;
box-shadow:
  0 20px 60px rgba(254, 126, 96, 0.15),
  0 4px 16px rgba(0, 0, 0, 0.08);
```

- Fondo del mockup: gradiente coral (#FFF5F3 → #FFE8E3)
- El dispositivo tiene bordes redondeados pronunciados (border-radius: 40px en el device)
- Sombra con tinte coral, no gris neutro

---

## Iconografía

### Estilo de íconos

- **Stroke (línea)**: peso de trazo 1.5–2px, no fill sólido
- **Tamaño base**: 20×20px en UI, 24×24px en hero/features
- **Color activo**: `#FE7E60`
- **Color inactivo**: `#474542` al 60% de opacidad
- **Fondo de ícono en tarjeta**: círculo `#FFF5F3`, 40–48px diámetro

### Categorías de íconos en la app

| Categoría        | Ícono sugerido  | Color de fondo   |
|------------------|-----------------|------------------|
| Vuelos           | avión           | `#FFF5F3`        |
| Hospedaje        | casa/cama       | `#FFF5F3`        |
| Bus / Tren       | transporte      | `#FFF5F3`        |
| Atracción        | ticket/estrella | `#EEE8AD` (20%)  |
| Restaurante      | tenedor         | `#FEB793` (20%)  |
| Pasaporte        | documento       | `#FFF5F3`        |
| Asistente IA     | chat/bot        | gradiente coral  |

---

## Logo

### Descripción

El logo de Navia es una combinación de **ícono + wordmark**:

**Ícono (maleta con flecha de navegación)**
- Forma: cuadrado redondeado (maleta de viaje) con asa visible en la parte superior
- Color: `#FE7E60` coral
- Interior: flecha de navegación / paper plane en blanco
- El ícono comunica "viaje" + "navegación/dirección" en una sola forma

**Wordmark**
- Texto: **"navia"** en minúsculas
- Tipografía: sans-serif bold (Outfit 700 o similar — redondeado, friendly)
- Color: `#1A1A1A` (versión principal)

**Tagline** (uso en versión extendida)
- "Tu viaje, en un solo lugar"
- Tipografía: DM Sans 400, gris `#474542`

### Archivos disponibles

| Archivo                          | Uso                                           |
|----------------------------------|-----------------------------------------------|
| `logo-navia.png`                 | Original PNG de alta resolución (3120×1755)   |
| `logo-navia-color.svg`           | Ícono coral + wordmark negro — navbar principal|
| `logo-navia-white.svg`           | Ícono blanco + wordmark blanco — sobre fondos oscuros o coral |
| `logo-navia-dark.svg`            | Ícono negro + wordmark negro — impresión       |
| `logo-icon-only.svg`             | Solo el ícono — favicons, app icon, avatares   |
| `favicon.png`                    | Favicon para web                               |

### Espacio de protección

Mínimo 16px de espacio libre alrededor del logo en todos los lados.

### Tamaño mínimo

- Digital: 80px de ancho para el wordmark completo; 32px para el ícono solo
- Print: 25mm de ancho

---

## Fotografía

Navia **no usa fotografía de personas en sus materiales principales**. El producto (app) es el protagonista visual.

Si se usa fotografía como contexto:
- Personas viajando con su teléfono (no mirando la cámara)
- Destinos internacionales con paleta cálida (dorados, corales, cielos)
- **Evitar**: personas en oficina, aeropuertos vacíos genéricos, imágenes de stock corporativas

---

## Qué NO hacer

- ❌ No usar íconos filled/sólidos — el estilo es stroke
- ❌ No usar paleta azul/corporate en ilustraciones — la marca es warm, no tech-blue
- ❌ No usar sombras neutras grises en mockups — usar sombras con tinte coral
- ❌ No mostrar la app con datos de ejemplo sin limpiar (nombres reales, info confidencial)
- ❌ No escalar el logo de forma no uniforme
- ❌ No colocar el logo coral sobre fondo coral
