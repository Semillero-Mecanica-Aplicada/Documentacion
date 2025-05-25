# Semillero de Investigación en Mecánica Aplicada


Repositorio oficial del <strong>Semillero de Investigación en Mecánica Aplicada</strong> — Proyecto 2025.

## 🚀 ¿Cómo subir un post?

1. **Ubica la carpeta de posts:**
   - Todos los posts están en la carpeta [`_posts/`](./_posts/).

2. **Crea un archivo Markdown:**
   - El nombre debe tener el formato: `AAAA-MM-DD-titulo-del-post.md`
   - Ejemplo: `2025-05-25-mi-nuevo-post.md`

3. **Agrega el front matter y contenido:**
   ```markdown
   ---
   title: Título del post
   tags: [Etiqueta1, Etiqueta2]
   ---
   
   Aquí va el contenido del post. Puedes usar **negritas**, _cursivas_, listas, imágenes, ecuaciones, etc.
   
   - Punto 1
   - Punto 2
   
   <!--more-->
   
   Texto que aparecerá después del resumen.
   ```

4. **Guarda y sube los cambios:**
   - Guarda el archivo en [`_posts/`](./_posts/).
   - Realiza commit y push a tu rama en el repositorio.

5. **Verifica el resultado:**
   - Inicia el servidor local:
     ```bash
     bundle exec jekyll serve
     ```
   - Abre [http://localhost:4000](http://localhost:4000) y revisa tu post.

## 📁 Estructura principal

- [`_posts/`](./_posts/): Posts del blog
- [`_data/`](./_data/): Archivos de configuración y datos
- [`_includes/`](./_includes/): Fragmentos HTML reutilizables
- [`_layouts/`](./_layouts/): Plantillas de página
- [`assets/`](./assets/): Imágenes, CSS y otros recursos
- [`index.html`](./index.html): Página principal

## 🛠️ Requisitos para desarrollo

- [Ruby](https://www.ruby-lang.org/)
- [Bundler](https://bundler.io/)
- [Jekyll](https://jekyllrb.com/)

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Abre un issue o pull request para sugerencias o mejoras.

---

