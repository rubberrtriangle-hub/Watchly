# Publicar Watchly en GitHub Pages

El objetivo es que la página quede accesible en:

https://rubberrtriangle-hub.github.io/Watchly/

y que esta URL abra directamente la sección "Cómo funciona":

https://rubberrtriangle-hub.github.io/Watchly/#how-it-works

## 1. Copiar los archivos al repositorio

En el repositorio `rubberrtriangle-hub/Watchly`, deja `index.html` en la raíz:

```text
Watchly/
├── index.html
├── privacy.html
├── README.md
└── assets/
    ├── styles.css
    └── favicon.svg
```

## 2. Activar GitHub Pages

En GitHub:

Settings → Pages

En "Build and deployment":

- Source: Deploy from a branch
- Branch: `main`
- Folder: `/ (root)`

Guarda los cambios.

## 3. Esperar la publicación

GitHub Pages generará:

https://rubberrtriangle-hub.github.io/Watchly/

La sección ya existe en `index.html` como:

```html
<section class="section section-dark" id="how-it-works">
```

Por eso esta URL funciona directamente:

https://rubberrtriangle-hub.github.io/Watchly/#how-it-works

## 4. Importante sobre el fragmento

La parte `#how-it-works` no es una página independiente. Es un fragmento de la misma `index.html` y hace que el navegador se desplace automáticamente hasta esa sección.

No hay que crear un archivo llamado `how-it-works.html`.
