# Portafolio — Kevin Cabrera

Página personal (una sola página, bilingüe ES/EN, tema claro/oscuro).

## Estructura

```
portfolio/
├── index.html          # la página
├── Styles/
│   └── Style.css       # estilos
├── assets/
│   └── photo.jpg       # foto de perfil
└── README.md
```

## Desplegar en GitHub Pages

### Opción A — subiendo por la web (sin comandos)
1. Crea un repositorio nuevo en GitHub (ej. `kncag.github.io` o `portafolio`).
2. Arrastra **el contenido** de esta carpeta (index.html, Styles/, assets/) al repo → *Commit changes*.
3. En el repo: **Settings → Pages**.
4. En *Build and deployment* → *Source*: **Deploy from a branch**.
5. *Branch*: `main` y carpeta `/ (root)` → **Save**.
6. Espera ~1 min y abre la URL que aparece (`https://kncag.github.io/<repo>/`).

> Si nombras el repo exactamente `kncag.github.io`, la página vivirá en `https://kncag.github.io/`.

### Opción B — por línea de comandos (git)
```bash
cd portfolio
git init
git add .
git commit -m "Portafolio personal"
git branch -M main
git remote add origin https://github.com/kncag/<repo>.git
git push -u origin main
```
Luego activa Pages igual que en la Opción A (pasos 3–6).

## Notas
- El botón **Descargar CV** abre el diálogo de impresión del navegador con un estilo limpio (Guardar como PDF). Cuando tengas un PDF propio, reemplázalo por un enlace: en `index.html` cambia el `<button id="cv-btn">` por `<a class="btn btn-outline" href="./assets/CV.pdf" download>…</a>` y coloca `CV.pdf` en `assets/`.
- El idioma y el tema se recuerdan en el navegador (localStorage).
- Las fuentes se cargan desde Google Fonts (requiere conexión).
