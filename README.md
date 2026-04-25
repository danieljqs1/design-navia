# Navia Design System v1.0.0

Plataforma de itinerarios inteligentes y asistente IA para agencias de viaje.

**Tagline:** Tu viaje, en un solo lugar.

---

## TL;DR — Valores clave

| Atributo          | Valor                                                             |
|-------------------|-------------------------------------------------------------------|
| **Color primario** | `#FE7E60` — coral principal (logo, CTAs, íconos activos)        |
| **Color hover**   | `#FE918B` — coral suave (gradiente de botón)                     |
| **Color accent**  | `#FEB793` — peach (secciones, fondos cálidos)                    |
| **Success**       | `#00BF63` — verde (confirmaciones, estado "Listo")               |
| **Text primary**  | `#1A1A1A` — headings                                             |
| **Text secondary**| `#474542` — body text                                            |
| **Fondo hero**    | `linear-gradient(135deg, #FFF → #FFE8E3 → #FEB793)`             |
| **Font display**  | `Outfit` 700/800 — headings, stats                               |
| **Font body**     | `DM Sans` 400/500/600 — UI, body text, botones                   |
| **Border radius** | `100px` (pills/botones) · `20px` (cards) · `12px` (íconos)      |
| **CTA principal** | "Solicitar acceso anticipado" → formulario de waitlist           |
| **Fundadora**     | Larissa Leal                                                     |

---

## Estructura del design system

```
design-navia/
├── README.md             ← este archivo
├── brand.md              ← misión, visión, audiencias, CTAs, diferenciadores
├── voice-and-tone.md     ← voz de marca, vocabulario, do/don't
├── colors.md             ← paleta completa + WCAG + combos aprobados
├── typography.md         ← familias, jerarquía, CSS import
├── imagery.md            ← dirección de arte, íconos, logo, mockups
├── components.md         ← CSS real para hero, nav, botones, cards, footer
├── tokens.json           ← fuente de verdad (formato DTCG W3C)
├── tokens.css            ← CSS custom properties listas para importar
└── Navia.pptx            ← material fuente de referencia
```

---

## Cómo usar este design system

### 1. Importar tokens en tu proyecto

```html
<link rel="stylesheet" href="tokens.css">
```

O en CSS:
```css
@import 'tokens.css';
```

### 2. Usar los tokens

```css
.my-button {
  background: var(--gradient-cta);
  color: var(--color-neutral-0);
  font-family: var(--font-body);
  font-weight: var(--weight-semibold);
  border-radius: var(--radius-full);
  padding: 14px var(--space-7);
  box-shadow: var(--shadow-btn-primary);
}
```

### 3. Fuentes (Google Fonts)

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=DM+Sans:ital,opsz,wght@0,9..40,400;0,9..40,500;0,9..40,600&display=swap" rel="stylesheet">
```

---

## Paleta rápida

```
Coral primario   ████  #FE7E60
Coral claro      ████  #FE918B
Peach            ████  #FEB793
Crema amarilla   ████  #EEE8AD
Fondo warm       ████  #FFF5F3
Verde éxito      ████  #00BF63
Text dark        ████  #1A1A1A
Text secondary   ████  #474542
```

---

## Principios de diseño

1. **Cálido, no genérico** — el coral y el peach definen la identidad; evitar azules corporativos
2. **Producto es el hero** — mockups de la app son el activo visual principal
3. **Espacio generoso** — mínimo 80px de padding vertical entre secciones
4. **Datos > promesas** — siempre anclar con números reales: 70%, <2 min, 24/7
5. **Stroke, no fill** — íconos con trazo, no sólidos
