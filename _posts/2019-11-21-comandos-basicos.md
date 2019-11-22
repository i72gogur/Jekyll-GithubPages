---
layout: post
author: rafa
---
A continuación se muestra un resumen de los comandos básicos que hemos utilizado para el desarrollo de nuestro proyecto.

1. Instalar ruby: `sudo apt-get install ruby-full build-essential zlib1g-dev`

2. Instalar gestor de gemas: `gem install bundler`

3. Instalar Jekyll: `gem install jekyll bundler`

4. Generar un nuevo sitio: `jekyll new NombreDelSitio`

5. Compilar el sitio para ser servido: `jekyll build`

6. Servir el sitio en local: `bundle exec jekyll serve`

---

## **COMANDOS PARA TRABAJAR CON GIT:**

1. Iniciar un repositorio: `git init`

2. Enlazar un directorio local con un repositorio de GitHub: `git remote add origin UrlDelRepositorio`

3. Crear una nueva rama: `git checkout -b NombreDeRama`

4. Añadir todos los archivos al repositorio: `git add .` ó `git add --all`

5. Hacer commit de los cambios realizados: `git commit -m "Mensaje"`

6. Subir el contenido actualizado al repositorio: `git push origin NombreDeRama`

7. Descargar el contenido desde el repositorio al directorio local: `git pull`