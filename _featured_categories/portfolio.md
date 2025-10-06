---
# Featured tags need to have either the `list` or `grid` layout (PRO only).
layout: list

# The title of the tag's page.
title: Portfolio

# The name of the tag, used in a post's front matter (e.g. tags: [<slug>]).
slug: project

# (Optional) Write a short (~150 characters) description of this featured tag.
description: >
  This is a featured category, which have their own page.
  Check out `_featured_tags/example.md` to learn how to create your own.

# (Optional) You can disable grouping posts by date.
# no_groups: true

# Exclude this example category from the sitemap.
# DON'T USE THIS SETTING IN YOUR CATEGORIES!
sitemap: false
---
<!--
--------------------------------------------------------------------------------
                    Prueba de tabla con codigo de chatgpt
--------------------------------------------------------------------------------
-->

# Tabla interactiva (HTML en Markdown)

Este archivo contiene un bloque de código HTML que muestra una tabla de 3 filas × 1 columna, sin bordes ni relleno en las celdas. La celda del medio contiene una imagen de ejemplo y toda la tabla es clicable (redirige a un enlace). Al poner el ratón encima, aparece un marco externo de una línea con bordes redondeados.

<!-- Sustituye el href y el src por tus propios valores -->
<div class="clickable-wrapper">
  <a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer" aria-label="Abrir enlace">
    <table class="no-style" role="presentation">
      <tbody>
        <tr>
          <td class="cell">Fila 1</td>
        </tr>
        <tr>
          <td class="cell center">
            <img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" />
          </td>
        </tr>
        <tr>
          <td class="cell">Fila 3</td>
        </tr>
      </tbody>
    </table>
  </a>
</div>

<style>
/* Contenedor clicable */
.clickable-wrapper {
  display: inline-block;
  border-radius: 12px;
  overflow: hidden; /* mantiene el zoom dentro */
  cursor: pointer;
  transition: box-shadow 200ms ease;
}

/* Sombra al hover */
.clickable-wrapper:hover {
  box-shadow: 0 10px 25px rgba(0,0,0,0.25);
}

/* Enlace base */
.clickable-link {
  display: block;
  text-decoration: none;
  color: inherit;
  outline: none;
}

/* Tabla sin bordes ni relleno */
.no-style {
  border-collapse: collapse;
  border-spacing: 0;
  margin: 0;
}
.no-style td {
  border: none;
  padding: 0;
}

/* Imagen centrada */
.cell.center { text-align: center; }
.cell.center img {
  display: block;
  max-width: 80%;
  height: auto;
  margin: 0 auto;
  transition: transform 250ms ease, filter 250ms ease;
}

/* Zoom solo en la imagen */
.clickable-wrapper:hover .cell.center img {
  transform: scale(1.05);
  filter: brightness(1.08);
}

/* Sin relleno adicional */
.cell { padding: 0; }

/* Foco accesible */
.clickable-link:focus-visible {
  outline: 3px solid rgba(21,156,228,0.6);
  outline-offset: 4px;
  border-radius: 8px;
}
</style>



<!--
--------------------------------------------------------------------------------
                          Prueba de next level tabla
--------------------------------------------------------------------------------
-->


<!--
Se hace una tabla que actua de galeria de 4x4 y dentro se mete cada una de las entradas que es
las tablas anteriores funcionales.
-->

<table class="outer-table" role="presentation">
  <tbody>
    <!-- 4 filas -->
    <tr>
      <!-- 4 columnas -->
      <td>
        <div class="clickable-wrapper">
          <a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer" aria-label="Abrir enlace">
            <table class="no-style" role="presentation">
              <tbody>
                <tr><td class="cell header"><strong>Fila 1</strong></td></tr>
                <tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr>
                <tr><td class="cell footer">Fila 3</td></tr>
              </tbody>
            </table>
          </a>
        </div>
      </td>
      <td>
        <div class="clickable-wrapper">
          <a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer" aria-label="Abrir enlace">
            <table class="no-style" role="presentation">
              <tbody>
                <tr><td class="cell header"><strong>Fila 1</strong></td></tr>
                <tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr>
                <tr><td class="cell footer">Fila 3</td></tr>
              </tbody>
            </table>
          </a>
        </div>
      </td>
      <td>
        <div class="clickable-wrapper">
          <a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer" aria-label="Abrir enlace">
            <table class="no-style" role="presentation">
              <tbody>
                <tr><td class="cell header"><strong>Fila 1</strong></td></tr>
                <tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr>
                <tr><td class="cell footer">Fila 3</td></tr>
              </tbody>
            </table>
          </a>
        </div>
      </td>
      <td>
        <div class="clickable-wrapper">
          <a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer" aria-label="Abrir enlace">
            <table class="no-style" role="presentation">
              <tbody>
                <tr><td class="cell header"><strong>Fila 1</strong></td></tr>
                <tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr>
                <tr><td class="cell footer">Fila 3</td></tr>
              </tbody>
            </table>
          </a>
        </div>
      </td>
    </tr>
    <!-- Duplica esta fila 3 veces más -->
    <tr>
      <td><div class="clickable-wrapper"><a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer"><table class="no-style"><tbody><tr><td class="cell header"><strong>Fila 1</strong></td></tr><tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr><tr><td class="cell footer">Fila 3</td></tr></tbody></table></a></div></td>
      <td><div class="clickable-wrapper"><a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer"><table class="no-style"><tbody><tr><td class="cell header"><strong>Fila 1</strong></td></tr><tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr><tr><td class="cell footer">Fila 3</td></tr></tbody></table></a></div></td>
      <td><div class="clickable-wrapper"><a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer"><table class="no-style"><tbody><tr><td class="cell header"><strong>Fila 1</strong></td></tr><tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr><tr><td class="cell footer">Fila 3</td></tr></tbody></table></a></div></td>
      <td><div class="clickable-wrapper"><a class="clickable-link" href="https://google.com" target="_blank" rel="noopener noreferrer"><table class="no-style"><tbody><tr><td class="cell header"><strong>Fila 1</strong></td></tr><tr><td class="cell center"><img src="/assets/img/blog/H101.png" alt="Imagen de ejemplo" /></td></tr><tr><td class="cell footer">Fila 3</td></tr></tbody></table></a></div></td>
    </tr>
    <!-- Repite dos veces más la fila anterior -->
  </tbody>
</table>

<style>
/* Tabla exterior 4x4 */
.outer-table {
  border-collapse: collapse;
  border-spacing: 0;
  width: 80%;              /* ocupa el 80% del ancho */
  margin: 0 auto;          /* centrada */
  text-align: center;
}
.outer-table td {
  width: 25%;              /* todas las celdas iguales */
  aspect-ratio: 1 / 1;     /* cuadradas */
  padding: 10px;
  border: none;
  background: none;
  vertical-align: middle;
}

/* Contenedor clicable */
.clickable-wrapper {
  display: inline-block;
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
  transition: box-shadow 200ms ease;
}

/* Sombra al hover */
.clickable-wrapper:hover {
  box-shadow: 0 10px 25px rgba(0,0,0,0.25);
}

/* Enlace base */
.clickable-link {
  display: block;
  text-decoration: none;
  color: inherit;
  outline: none;
}

/* Tabla interior sin bordes */
.no-style {
  border-collapse: collapse;
  border-spacing: 0;
  margin: 0;
  width: 100%;
  height: 100%;
}
.no-style td {
  border: none;
  padding: 0;
}

/* Texto centrado */
.cell.header, .cell.footer {
  text-align: center;
  font-family: sans-serif;
}
.cell.header { font-weight: bold; }

/* Imagen reducida */
.cell.center img {
  display: block;
  width: 80%;   /* 20% más pequeña */
  height: auto;
  margin: 0 auto;
  transition: transform 250ms ease, filter 250ms ease;
}

/* Zoom y brillo solo en imagen */
.clickable-wrapper:hover .cell.center img {
  transform: scale(1.05);
  filter: brightness(1.08);
}

/* Foco accesible */
.clickable-link:focus-visible {
  outline: 3px solid rgba(21,156,228,0.6);
  outline-offset: 4px;
  border-radius: 8px;
}
</style>


<!--
--------------------------------------------------------------------------------
                          Prueba de tabla optimizada
--------------------------------------------------------------------------------
-->


<!--
Le he pedido a chargpt que actualice la forma de trabajar y me ha dado este codigo, aun 
falta por refiniar para que su estructurea planteada encaje con la que ya hay
-->