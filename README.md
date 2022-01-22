Sitio web del Proyecto Alejandría
=================================

Desarrollado utilizando [Hugo](https://gohugo.io/), [Bootstrap 5](https://getbootstrap.com/) y [Font Awesome 5](https://fontawesome.com/).

Tema original de [StartBootstrap](https://github.com/StartBootstrap/startbootstrap-agency).

## Desarrollo

Para construir el sitio estático:

    hugo

Opcionalmente con la opción `--minify` para comprimir los ficheros resultantes.

Para servir el sitio localmente, con re-compilación y recarga automática:

    hugo serve -D

## Despliegue continuo

El sitio se construye y despliega en [GitHub Pages](https://pages.github.com/) utilizando [GitHub Actions](https://docs.github.com/en/actions). El flujo está definido en [.github/workflows/gh-pages.yml](.github/workflows/gh-pages.yml) y se puede resumir en estas acciones:

1. Obtener el árbol de ficheros del repositorio.
2. Cargar la última versión de _Hugo_.
3. Construir el sitio con _Hugo_.
4. Subir el sitio a la rama `gh-pages`.

Es posible realizar un despliegue manual haciendo _push_ a la rama `gh-pages`.
