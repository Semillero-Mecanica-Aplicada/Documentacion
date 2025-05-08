# Semillero de Investigación en Mecánica Aplicada – Proyecto 2025

Bienvenidos al repositorio oficial del Semillero de Investigación en Mecánica Aplicada. Este espacio está destinado a documentar semana a semana el desarrollo del proyecto 2025, incluyendo reuniones, avances técnicos, resultados y recursos clave.

---

## 📁 Estructura del repositorio

```
/
├── index.md                 # Página principal del sitio
├── blog.html                # Página tipo blog que lista las actas
├── _posts/                  # Carpeta donde se colocan las actas semanales en formato Markdown
│   ├── 2025-03-17-charla-elasticidad.md
├── _layouts/
│   └── default.html         # Plantilla base del sitio
├── _config.yml              # Configuración general del sitio Jekyll
└── README.md                # Este archivo
```

---

## 🔧 ¿Cómo colaborar?

### 1. Clona el repositorio

```bash
git clone https://github.com/Semillero-Mecanica-Aplicada/Documentacion.git
cd Documentacion
```

### 2. Agrega una nueva acta semanal

1. Crea un nuevo archivo en la carpeta `_posts/` siguiendo este formato de nombre:

```
YYYY-MM-DD-nombre-del-acto.md
```

2. Dentro del archivo, usa esta plantilla:

```markdown
---
layout: post
title: Semana X - Título de la reunión
date: YYYY-MM-DD
---

**Fecha:** DD de mes de 2025

**Temas tratados:**

- Punto 1 tratado en la reunión
- Punto 2 tratado en la reunión
- Punto 3 tratado en la reunión

**Responsables:** Nombre 1, Nombre 2

**Próximos pasos:** Actividades asignadas para la próxima semana.
```

> ✅ Puedes escribir todo en formato Markdown. Jekyll se encargará de convertirlo en una página web automáticamente.

### 3. Guarda y sube los cambios

```bash
git add .
git commit -m "Agregada acta semana X"
git push origin main
```

---

## 🌐 ¿Cómo ver la página en línea?

GitHub Pages está activado para este repositorio.

Puedes visitar la página principal en:

```
https://semillero-mecanica-aplicada.github.io/Documentacion/
```

Y la documentación directamente en:

```
https://semillero-mecanica-aplicada.github.io/Documentacion/blog.html
```

---

## 📫 Contacto

Para dudas, errores o mejoras, contacta al coordinador del semillero o abre un Issue en este repositorio.

---

© 2025 – Semillero de Investigación en Mecánica Aplicada
