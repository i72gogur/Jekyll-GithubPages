---
layout: post
author: rafa
---

Desplegar tu sitio para que cualquiera pueda visitarlo es muy simple gracias a Jekyll y Github-Pages. Tan solo tienes que seguir estos pasos:

1. Editar el archivo de configuración _config.yml, modificando los parámetros baseurl donde añadiremos el nombre del repositorio desde el que accederemos a nuestro sitio y el parámetro url con la dirección completa de nuestro sitio.
En nuestro caso será: https://i72gogur.github.io/Jekyll-GithubPages

2. Iniciamos git en un directorio local con: `git init`

3. Enlazamos el repositorio de git con nuestro directorio local: `git remote add origin https://github.com/i72gogur/NombreDelRepositorio.git`

4. Creamos una nueva rama para Github-Pages: `git checkout -b gh-pages`

5. Añadimos todos los archivos: `git add .`

6. Hacemos commit: `git commit -m "Mensaje"`

7. Subimos el contenido a la rama creada con: `git push origin gh-pages`

8. Vamos al apartado de configuración desde nuestro repositorio git y desde la opción de Github Pages seleccionamos la opción de utilizar la rama que hemos creado (gh-pages)

9. ¡Y listo! Nuestro sitio estará disponible [aquí](https://i72gogur.github.io/Jekyll-GithubPages)