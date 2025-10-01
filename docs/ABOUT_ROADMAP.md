# 🗺️ Roadmap – About Page (v1)

Este documento define los pasos para dejar lista la primera versión del About Page antes de hacer merge a `develop`.

---

## 1. Contenido base
- [ ] Crear archivo `content/about.md`.  
- [ ] Redactar bio corta (100–150 palabras) → formación, experiencia y visión LATAM.  
- [ ] Incluir foto/avatar (`static/images/mike.png`).  

---

## 2. Estructura visual
- [ ] Usar layout de página simple de PaperMod.  
- [ ] Título visible: *Sobre mí*.  
- [ ] Texto alineado + imagen (layout centrado o lado a lado).  
- [ ] Botón/CTA → “Conecta en LinkedIn” o “Descarga mi CV”.  

---

## 3. Integración en el sitio
- [ ] Validar que el menú “Sobre mí” redirija correctamente a `/about/`.  
- [ ] Ajustar estilos mínimos en `customCSS/global.css` (márgenes, tipografía, foto redondeada).  
- [ ] Probar en local con `hugo server -D`.  

---

## 4. Preparación para commit
- [ ] Revisar que el texto esté alineado al tono profesional (consultoría IA + research).  
- [ ] Confirmar que la imagen carga correctamente.  
- [ ] `git add content/about.md static/images/mike.png`.  
- [ ] `git commit -m "feat: add initial about page v1"`.  
- [ ] Push a branch `feature/about-page`.  

---

## 5. Iteración futura (v2)
- [ ] Expandir con línea de tiempo (formación, proyectos, publicaciones).  
- [ ] Añadir sección bilingüe (EN/ES).  
- [ ] Embeds (papers, charlas, conferencias).  
- [ ] Versión descargable en PDF (CV/portfolio).  

---

📌 **Estado actual:** 0% → por iniciar.  
**Pendiente clave:** Crear `content/about.md` con la primera bio.  
