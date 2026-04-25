# Navia — Colors

## Paleta completa

### Brand / Coral

| Token                  | HEX       | RGB              | Rol                                          |
|------------------------|-----------|------------------|----------------------------------------------|
| `--color-brand-600`    | `#FE7E60` | 254, 126, 96     | **Primary** — botones CTA, íconos activos, logo |
| `--color-brand-400`    | `#FE918B` | 254, 145, 139    | Hover de botón, gradiente CTA                |
| `--color-brand-300`    | `#FEB793` | 254, 183, 147    | Peach accent — fondo secciones, tarjetas      |
| `--color-brand-100`    | `#FFE8E3` | 255, 232, 227    | Background coral suave                        |
| `--color-brand-50`     | `#FFF5F3` | 255, 245, 243    | Background casi blanco con tinte cálido       |

### Accent / Amarillo crema

| Token                  | HEX       | RGB              | Rol                                          |
|------------------------|-----------|------------------|----------------------------------------------|
| `--color-accent-200`   | `#EEE8AD` | 238, 232, 173    | Accent secundario — categorías, tags          |

### Success / Verde

| Token                  | HEX       | RGB              | Rol                                          |
|------------------------|-----------|------------------|----------------------------------------------|
| `--color-success-500`  | `#00BF63` | 0, 191, 99       | Confirmaciones, estados activos, "Listo"     |
| `--color-success-100`  | `#CDE9BF` | 205, 233, 191    | Fondo de éxito suave, badges verdes          |

### Neutral / Texto

| Token                  | HEX       | RGB              | Rol                                          |
|------------------------|-----------|------------------|----------------------------------------------|
| `--color-neutral-900`  | `#1A1A1A` | 26, 26, 26       | Headings principales                         |
| `--color-neutral-700`  | `#474542` | 71, 69, 66       | Body text, textos secundarios                |
| `--color-neutral-0`    | `#FFFFFF` | 255, 255, 255    | Fondos de tarjetas, nav, contenedores        |

---

## Gradientes

```css
/* Hero background — uso en pantalla completa */
background: linear-gradient(135deg, #FFFFFF 0%, #FFE8E3 50%, #FEB793 100%);

/* CTA button — botón primario */
background: linear-gradient(to right, #FE7E60 0%, #FE918B 100%);

/* Card warm — fondo de tarjetas de feature */
background: linear-gradient(to bottom right, #FFF5F3 0%, #FFFFFF 100%);

/* Gradient peach-yellow — secciones de categorías */
background: linear-gradient(to bottom right, #FEB793 0%, #EEE8AD 100%);

/* Dark subtle — footer o secciones oscuras */
background: linear-gradient(to bottom right, #474542 0%, #2D2B28 100%);
```

---

## Combos aprobados

### Hero principal
```
fondo:      linear-gradient(135deg, #FFFFFF → #FFE8E3 → #FEB793)
heading:    #1A1A1A  (Outfit 600)
accent:     #FE7E60  (palabra clave en el heading)
subtítulo:  #474542  (DM Sans regular)
CTA:        #FE7E60 → #FE918B (pill, degradado)
```

### Card de feature
```
fondo:      #FFFFFF con borde rgba(254,126,96,0.1)
ícono:      #FE7E60 sobre fondo #FFF5F3
título:     #1A1A1A  (Outfit 600)
descripción:#474542  (DM Sans 400)
```

### Comparativa ANTES/CON NAVIA
```
columna ANTES:    fondo #F5F5F5, texto #474542, ícono gris
columna CON NAVIA: fondo gradiente coral, texto #1A1A1A, check #00BF63
```

### Estado de éxito / confirmación
```
fondo:  #CDE9BF
texto:  #1A1A1A
ícono:  #00BF63
```

### Estadísticas (números grandes)
```
número:     #FE7E60  (Outfit 700, 48–64px)
etiqueta:   #474542  (DM Sans 400, 14px)
fondo:      #FFFFFF
```

---

## Contraste WCAG

| Combinación                        | Ratio   | Nivel    |
|------------------------------------|---------|----------|
| `#1A1A1A` sobre `#FFFFFF`          | 18.1:1  | AAA ✅   |
| `#1A1A1A` sobre `#FFF5F3`          | 17.2:1  | AAA ✅   |
| `#474542` sobre `#FFFFFF`          | 8.9:1   | AAA ✅   |
| `#474542` sobre `#FFF5F3`          | 8.4:1   | AAA ✅   |
| `#FFFFFF` sobre `#FE7E60`          | 3.1:1   | AA (lg)✅|
| `#1A1A1A` sobre `#FEB793`          | 7.2:1   | AAA ✅   |
| `#FFFFFF` sobre `#1A1A1A`          | 18.1:1  | AAA ✅   |

---

## Qué NO hacer

- ❌ No usar `#FE7E60` como color de texto sobre fondo blanco — contraste insuficiente para body text
- ❌ No combinar `#FEB793` con `#EEE8AD` como texto sobre fondo — demasiado bajo contraste
- ❌ No usar verde `#00BF63` como color de acción primaria — está reservado exclusivamente para estados de éxito
- ❌ No usar más de 2 colores de la paleta brand en una misma tarjeta
- ❌ No crear fondos completamente negros o navy — la marca es cálida, no dark mode por defecto
- ❌ No mezclar el gradiente hero con la paleta green — son mundos visuales distintos
