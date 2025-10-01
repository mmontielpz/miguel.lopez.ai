# 🗺️ Roadmap – Portfolio Page (v1)

Guía para construir la primera versión de la página **Portafolio** antes de hacer merge a `develop` y luego a `main`.

---

## 🎯 Objetivo
Mostrar 3 proyectos representativos que demuestren resultados e impacto (industria & research) con una presentación clara y coherente con el branding del sitio.

---

## ✅ Entregables v1
- [x] Página de sección en `/portfolio/` (Hugo + PaperMod).  
- [x] 3 proyectos con: título, sector, rol, breve descripción (2–3 líneas), resultado/impacto.  
- [x] Estilos consistentes con las *cards* de “Servicios”.  
- [x] Links funcionales solo en Research (Springer, SPIE).  
- [ ] Preparar merge a `develop`.  

---

## 1) Contenido base
- [x] Crear carpeta y archivo: `content/portfolio/_index.md`.  
- [x] Definir 3 proyectos (Healthcare – Document Intelligence, Manufacturing – Predictive Maintenance, Research – Springer/SPIE).  
- [x] Redactar descripciones cortas enfocadas en **beneficio/impacto** (cualitativo, sin métricas).  
- [ ] Revisar si conviene expandir a 4 proyectos en v1 (ej. un demo propio o hackathon).  

---

## 2) Estructura visual
- [x] Usar **grid de cards** (similar a Servicios).  
- [x] Cada card: título → sector/rol → descripción → impacto → CTA (solo en Research).  
- [x] Tipografías y espaciados consistentes con `global.css`.  
- [x] Responsivo probado en móvil y desktop.  

---

## 3) Integración en el sitio
- [x] Validar item de menú “Portafolio” → `/portfolio/`.  
- [x] Ajustar estilos mínimos en `assets/css/global.css` (`.portfolio-grid`, `.btn-secondary`).  
- [x] Probar en local: `hugo server -D`.  

---

## 4) QA & Accesibilidad
- [ ] Añadir `alt` en imágenes si en el futuro se incluyen capturas/screenshots.  
- [x] Verificar que links externos abren en nueva pestaña.  
- [x] Revisar comportamiento móvil (grid → 1 columna).  

---

## 5) SEO / Metadatos
- [x] `title` y `description` en el front matter de `_index.md`.  
- [ ] OpenGraph básico (usar imagen genérica de portafolio si no hay capturas).  
- [ ] Preparar metadatos por proyecto cuando existan páginas detalle.  

---

## 6) Preparación para PR
- [x] `git add content/portfolio/_index.md assets/css/global.css`.  
- [ ] `git commit -m "feat(portfolio): add portfolio page v1 with project cards"`.  
- [ ] Abrir PR: `feature/portfolio-page` → `develop`.  

---

## (v2) Iteración futura
- [ ] Imágenes/screenshots por proyecto (optimizar peso).  
- [ ] Filtros por categoría (*Industry | Research | Publications*).  
- [ ] Páginas detalle por proyecto (`/portfolio/<slug>/`) con métricas y stack técnico.  
- [ ] CTA final: “¿Quieres un caso similar? Contáctame”.  
- [ ] OpenGraph mejorado con previews de proyectos.  
- [ ] Estadísticas de engagement (clicks, scroll) con simple analytics.  

---

## ✅ Definition of Done (v1)
- Navegable desde el menú.  
- 3 proyectos visibles en grid, con CTA funcional (Research).  
- Responsive y accesible en móvil.  
- Build local OK y PR listo a `develop`.  
