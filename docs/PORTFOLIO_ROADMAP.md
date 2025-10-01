# 🗺️ Roadmap – Portfolio Page (v1)

Guía para construir la primera versión de la página **Portafolio** antes de hacer merge a `develop` y luego a `main`.

---

## 🎯 Objetivo
Mostrar 3–4 proyectos representativos que demuestren resultados e impacto (industria & research) con una presentación clara y coherente con el branding del sitio.

---

## ✅ Entregables v1
- Página de sección en ` /portfolio/ ` (Hugo + PaperMod).
- 3–4 proyectos con: título, sector, rol, breve descripción (2–3 líneas), resultado/impacto y CTA (link externo o interno).
- Estilos consistentes con las *cards* de “Servicios”.

---

## 1) Contenido base
- [ ] Crear carpeta y archivo: `content/portfolio/_index.md`.
- [ ] Definir 3–4 proyectos (ej. Illumina – Document Intelligence, Manufactura – Predictive Maintenance, Publicaciones – Springer/SPIE).
- [ ] Redactar descripciones cortas enfocadas en **beneficio/impacto**.
- [ ] Agregar enlaces (paper, repo, artículo o nota interna futura).

---

## 2) Estructura visual
- [ ] Usar **grid de cards** (similar a Servicios).
- [ ] Cada card: **título → sector/rol → descripción → resultado → CTA**.
- [ ] Mantener tipografías y espaciados del sitio (usar variables de `global.css`).
- [ ] Responsivo: 1 col (móvil), 2–3 cols (tablet/desktop).

---

## 3) Integración en el sitio
- [ ] Validar item de menú “Portafolio” → `/portfolio/` (ya existe en `config.toml`).
- [ ] Ajustar estilos mínimos en `assets/css/global.css` (si hace falta clase `.portfolio-grid`).
- [ ] Probar en local: `hugo server -D` → `http://localhost:1313/miguel.lopez.ai/portfolio/`.

---

## 4) QA & Accesibilidad
- [ ] Revisar contraste, tamaño de fuente y `alt` en imágenes (si se añaden).
- [ ] Verificar links (que abran en pestaña nueva si son externos).
- [ ] Checar comportamiento móvil (saltos de línea y márgenes).

---

## 5) SEO / Metadatos
- [ ] `title` y `description` en el front matter de `_index.md`.
- [ ] OpenGraph básico (usar imagen genérica si no hay screenshots de proyectos).
- [ ] Slugs legibles si luego se crean páginas por proyecto (`/portfolio/illumina/`, etc.).

---

## 6) Preparación para PR
- [ ] `git add content/portfolio/_index.md assets/css/global.css`.
- [ ] `git commit -m "feat(portfolio): add portfolio page v1 (projects grid + copy)"`.
- [ ] Abrir PR: `feature/portfolio-page` → `develop`.

---

## (v2) Iteración futura
- [ ] Imágenes/screenshots por proyecto (optimizar peso).
- [ ] Filtros por categoría (*Industry | Research | Publications*).
- [ ] Páginas detalle por proyecto (`/portfolio/<slug>/`) con métricas y stack técnico.
- [ ] CTA final: “¿Quieres un caso similar? Contáctame”.
- [ ] Estadísticas de engagement (clicks, scroll) con simple analytics.

---

## ✅ Definition of Done (v1)
- Navegable desde el menú.
- 3–4 proyectos visibles en grid, con CTA funcional.
- Responsive y accesible en móvil.
- Build local OK y PR listo a `develop`.
