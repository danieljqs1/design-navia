# Navia — Typography

## Familias tipográficas

| Rol          | Familia    | Fuente             | Uso                                      |
|--------------|------------|--------------------|------------------------------------------|
| Display      | `Outfit`   | Google Fonts       | Headings H1–H3, números estadísticos     |
| Body         | `DM Sans`  | Google Fonts       | Body text, UI labels, captions           |
| Fallback     | `sans-serif` | Sistema          | Respaldo universal                       |

---

## Import CSS

```css
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600&display=swap');
```

---

## Jerarquía tipográfica

### Display — Outfit

| Nivel        | Font         | Weight | Size          | Line Height | Uso                             |
|--------------|--------------|--------|---------------|-------------|---------------------------------|
| `display-xl` | Outfit       | 800    | 56–72px       | 1.05        | Hero H1 — frase de impacto      |
| `heading-1`  | Outfit       | 700    | 40–48px       | 1.1         | Títulos de sección principales  |
| `heading-2`  | Outfit       | 600    | 28–32px       | 1.2         | Subtítulos de sección           |
| `heading-3`  | Outfit       | 600    | 20–24px       | 1.3         | Títulos de tarjetas             |
| `stat`       | Outfit       | 700    | 48–56px       | 1.0         | Números estadísticos (70%, <2min) |

### Body — DM Sans

| Nivel        | Font         | Weight | Size     | Line Height | Uso                               |
|--------------|--------------|--------|----------|-------------|-----------------------------------|
| `body-lg`    | DM Sans      | 400    | 18px     | 1.6         | Párrafo principal, descripción    |
| `body-md`    | DM Sans      | 400    | 16px     | 1.6         | Body text estándar                |
| `body-sm`    | DM Sans      | 400    | 14px     | 1.5         | Captions, labels UI               |
| `label`      | DM Sans      | 500    | 14px     | 1.4         | Etiquetas de formulario, nav items|
| `button`     | DM Sans      | 600    | 15–16px  | 1.0         | Texto de botones                  |
| `caption`    | DM Sans      | 400    | 12px     | 1.4         | Notas legales, metadata           |

---

## Tamaños en escala (clamp responsive)

```css
--text-display-xl: clamp(40px, 5vw, 72px);
--text-h1:         clamp(32px, 4vw, 48px);
--text-h2:         clamp(24px, 3vw, 32px);
--text-h3:         clamp(18px, 2.5vw, 24px);
--text-stat:       clamp(36px, 4.5vw, 56px);
--text-body-lg:    18px;
--text-body-md:    16px;
--text-body-sm:    14px;
--text-caption:    12px;
```

---

## Ejemplos de uso en código

```css
/* Hero heading */
font-family: 'Outfit', sans-serif;
font-size: clamp(40px, 5vw, 72px);
font-weight: 700;
line-height: 1.05;
color: #1A1A1A;

/* Accent word in heading (coral) */
color: #FE7E60;

/* Body paragraph */
font-family: 'DM Sans', sans-serif;
font-size: 18px;
font-weight: 400;
line-height: 1.6;
color: #474542;

/* Button */
font-family: 'DM Sans', sans-serif;
font-size: 15px;
font-weight: 600;
letter-spacing: 0.01em;

/* Stat number */
font-family: 'Outfit', sans-serif;
font-size: clamp(36px, 4.5vw, 56px);
font-weight: 700;
color: #FE7E60;
```

---

## Qué NO hacer

- ❌ No usar Outfit para body text corrido — pierde legibilidad en textos largos
- ❌ No usar DM Sans en headings principales — carece del carácter display necesario
- ❌ No mezclar más de 2 familias en un mismo componente
- ❌ No usar font-weight 400 en Outfit para headings — usar mínimo 600
- ❌ No usar tamaños de heading fijos sin clamp en contextos responsive
- ❌ No usar letter-spacing negativo en Outfit — afecta legibilidad en weights altos
