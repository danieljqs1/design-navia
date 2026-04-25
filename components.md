# Navia — Components

## Botones

### Botón primario (CTA principal)

```html
<button class="btn-primary">Solicitar acceso anticipado</button>
```

```css
.btn-primary {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 14px 28px;
  background: linear-gradient(to right, #FE7E60 0%, #FE918B 100%);
  color: #FFFFFF;
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  font-weight: 600;
  letter-spacing: 0.01em;
  border: none;
  border-radius: 100px;
  cursor: pointer;
  transition: opacity 0.2s ease, transform 0.15s ease;
  box-shadow: 0 4px 16px rgba(254, 126, 96, 0.3);
}

.btn-primary:hover {
  opacity: 0.9;
  transform: translateY(-1px);
  box-shadow: 0 8px 24px rgba(254, 126, 96, 0.4);
}

.btn-primary:active {
  transform: translateY(0);
  opacity: 1;
}
```

### Botón secundario (outline / ghost)

```html
<button class="btn-secondary">Ver cómo funciona</button>
```

```css
.btn-secondary {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 13px 28px;
  background: transparent;
  color: #474542;
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  font-weight: 500;
  border: 1.5px solid rgba(71, 69, 66, 0.2);
  border-radius: 100px;
  cursor: pointer;
  transition: border-color 0.2s ease, color 0.2s ease;
}

.btn-secondary:hover {
  border-color: #FE7E60;
  color: #FE7E60;
}
```

---

## Navbar

```
┌─────────────────────────────────────────────────────────────┐
│  [navia]                              [Solicitar acceso →]  │
└─────────────────────────────────────────────────────────────┘
```

```css
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 40px;
  background: rgba(255, 255, 255, 0.85);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(254, 126, 96, 0.08);
  position: sticky;
  top: 0;
  z-index: 100;
}

.navbar-logo {
  font-family: 'Outfit', sans-serif;
  font-size: 20px;
  font-weight: 700;
  color: #FE7E60;
  text-decoration: none;
  letter-spacing: -0.02em;
}
```

---

## Hero Section

```
┌──────────────────────────────────────────────────────────────────┐
│  background: linear-gradient(135deg, #FFF → #FFE8E3 → #FEB793)  │
│                                                                   │
│  ┌──────────────────────────────────────────────────────────┐    │
│  │  [pill badge]  Acceso anticipado disponible              │    │
│  │                                                          │    │
│  │  Deja que la IA organice los                             │    │
│  │  viajes de tus clientes                                  │    │
│  │        ^^^^^^^^^^^^ (en coral #FE7E60)                   │    │
│  │                                                          │    │
│  │  Navia genera itinerarios inteligentes, tickets          │    │
│  │  digitales y un asistente virtual 24/7 — directo al      │    │
│  │  celular de tus viajeros.                                │    │
│  │                                                          │    │
│  │  [Solicitar acceso anticipado ↗]  [Ver cómo funciona]    │    │
│  └──────────────────────────────────────────────────────────┘    │
│                                                                   │
│  [ App dashboard mockup + iPhone mockup ]                        │
└──────────────────────────────────────────────────────────────────┘
```

```css
.hero {
  min-height: 100vh;
  background: linear-gradient(135deg, #FFFFFF 0%, #FFE8E3 50%, #FEB793 100%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding: 80px 40px 60px;
  text-align: center;
}

.hero-badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 16px;
  background: rgba(254, 126, 96, 0.1);
  border: 1px solid rgba(254, 126, 96, 0.2);
  border-radius: 100px;
  font-family: 'DM Sans', sans-serif;
  font-size: 13px;
  font-weight: 500;
  color: #FE7E60;
  margin-bottom: 24px;
}

.hero-heading {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(40px, 5vw, 72px);
  font-weight: 700;
  line-height: 1.05;
  color: #1A1A1A;
  max-width: 800px;
  margin-bottom: 24px;
}

.hero-heading .accent {
  color: #FE7E60;
}

.hero-body {
  font-family: 'DM Sans', sans-serif;
  font-size: 18px;
  font-weight: 400;
  line-height: 1.6;
  color: #474542;
  max-width: 560px;
  margin-bottom: 40px;
}

.hero-actions {
  display: flex;
  align-items: center;
  gap: 16px;
  flex-wrap: wrap;
  justify-content: center;
}
```

---

## Stats Bar

```
┌──────────────────────────────────────────────────────────┐
│   70%          24/7         <2 min          0            │
│   de viajeros  asistencia   para generar   llamadas      │
│   prefieren    sin inter-   un itinerario  a destiempo   │
│   digital      vención      completo                     │
└──────────────────────────────────────────────────────────┘
```

```css
.stats-bar {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 40px;
  padding: 48px 40px;
  background: #FFFFFF;
}

.stat-item {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 4px;
}

.stat-number {
  font-family: 'Outfit', sans-serif;
  font-size: clamp(36px, 4vw, 52px);
  font-weight: 700;
  color: #FE7E60;
  line-height: 1.0;
}

.stat-label {
  font-family: 'DM Sans', sans-serif;
  font-size: 14px;
  font-weight: 400;
  color: #474542;
  line-height: 1.4;
  max-width: 120px;
}
```

---

## Feature Card

```
┌────────────────────────────────┐
│  ┌────┐                        │
│  │ 🗂️ │  Itinerarios           │
│  └────┘  inteligentes          │
│                                │
│  Genera itinerarios en         │
│  segundos a partir de tus      │
│  documentos de reserva.        │
└────────────────────────────────┘
```

```css
.feature-card {
  background: linear-gradient(to bottom right, #FFF5F3 0%, #FFFFFF 100%);
  border: 1px solid rgba(254, 126, 96, 0.1);
  border-radius: 20px;
  padding: 28px;
  display: flex;
  flex-direction: column;
  gap: 16px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.feature-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 16px 40px rgba(254, 126, 96, 0.12);
}

.feature-icon-wrap {
  width: 48px;
  height: 48px;
  border-radius: 12px;
  background: #FFF5F3;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #FE7E60;
}

.feature-title {
  font-family: 'Outfit', sans-serif;
  font-size: 18px;
  font-weight: 600;
  color: #1A1A1A;
  line-height: 1.3;
}

.feature-description {
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  font-weight: 400;
  color: #474542;
  line-height: 1.6;
}
```

---

## Comparison Table (ANTES / CON NAVIA)

```
┌──────────────────────────┬──────────────────────────┐
│  ANTES                   │  CON NAVIA               │
├──────────────────────────┼──────────────────────────┤
│  ✗ Carpetas y papeles    │  ✓ Tickets digitales     │
│  ✗ Llamadas a destiempo  │  ✓ ChatBot IA 24/7       │
│  ✗ PDFs perdidos         │  ✓ Itinerario visual     │
└──────────────────────────┴──────────────────────────┘
```

```css
.comparison-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
  max-width: 800px;
  margin: 0 auto;
}

.comparison-col {
  border-radius: 20px;
  padding: 28px;
}

.comparison-col.before {
  background: #F5F4F2;
}

.comparison-col.with-navia {
  background: linear-gradient(135deg, #FE7E60 0%, #FE918B 50%, #FEB793 100%);
  color: #FFFFFF;
}

.comparison-label {
  font-family: 'DM Sans', sans-serif;
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  opacity: 0.6;
  margin-bottom: 16px;
}

.comparison-item {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  font-family: 'DM Sans', sans-serif;
  font-size: 15px;
  line-height: 1.5;
  padding: 8px 0;
  border-bottom: 1px solid rgba(0,0,0,0.06);
}

.comparison-col.with-navia .comparison-item {
  border-bottom-color: rgba(255,255,255,0.15);
}
```

---

## Footer

```
┌─────────────────────────────────────────────────────────────┐
│  [navia]                                                    │
│  Tu viaje, en un solo lugar.                                │
│                                                             │
│  © 2025 Navia. Todos los derechos reservados.              │
└─────────────────────────────────────────────────────────────┘
```

```css
.footer {
  background: linear-gradient(to bottom right, #474542 0%, #2D2B28 100%);
  color: #FFFFFF;
  padding: 48px 40px;
  display: flex;
  flex-direction: column;
  gap: 24px;
}

.footer-logo {
  font-family: 'Outfit', sans-serif;
  font-size: 22px;
  font-weight: 700;
  color: #FE7E60;
  letter-spacing: -0.02em;
}

.footer-tagline {
  font-family: 'DM Sans', sans-serif;
  font-size: 14px;
  color: rgba(255, 255, 255, 0.6);
}

.footer-copy {
  font-family: 'DM Sans', sans-serif;
  font-size: 12px;
  color: rgba(255, 255, 255, 0.4);
  padding-top: 16px;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
}
```

---

## Badge de estado (Success / Pending)

```css
.badge {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 4px 12px;
  border-radius: 100px;
  font-family: 'DM Sans', sans-serif;
  font-size: 12px;
  font-weight: 500;
}

.badge-success {
  background: #CDE9BF;
  color: #1A5C30;
}

.badge-pending {
  background: rgba(254, 183, 147, 0.3);
  color: #8B4513;
}

.badge-info {
  background: rgba(254, 126, 96, 0.1);
  color: #FE7E60;
}
```
