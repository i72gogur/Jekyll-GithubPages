---
layout: post
author: leo
---

Otro recurso que nos servirá de utilidad para la elaboración de nuestro sitio web son los assets, los cuales nos permitirán añadir fotos o archivos PDF a nuestros posts. Para ello crearemos una carpeta que con el nombre de assets y en la que incluiremos todas las imágenes o archivos que queremos que aparezcan en nuestra página. Además, también podemos añadir archivos de estilo css y nuestros scripts en javascript de esta forma, organizando la carpeta en subcarpetas tendremos todos los recursos bien organizados.
Después, para utilizarlos simplemente tendremos que enlazarlos añadiendo la ruta del archivo que queremos añadir en el código de nuestro post.

Por ejemplo, si queremos añadir la imagen de nuestro logotipo en lenguaje Markdown haríamos lo siguiente:

`![Logotipo](/assets/images/logotipo.png)`

La principal utilidad que tiene el uso de assets es a la hora de dar estilo a nuestra página, para ello podemos utilizar Sass que es un preprocesador de lenguaje para hojas de estilo y que podemos usar conjuntamente con CSS.

Primero crearemos un archivo Saas con extensión .scss, por ejemplo estilos.scss y lo añadiremos a nuestra carpeta de css dentro del directorio de assets. En este archivo dejaremos el front matter vacío, lo cual le indica a jekyll que tiene que procesar y añadiremos también la siguiente línea de código para importar el archivo de estilos, quedando nuestro archivos scss de la siguiente forma:

`---`  
`---`  
`@import "main";`

Con esto indicamos a Sass que busque un archivo llamado main.scss (que en nuestro caso contendrá el estilo de nuestra página principal) en el directorio correspondiente a los archivos Sass.

Por último, para usar esta hoja de estilos solamente tendremos que incluir en la cabecera del archivo html al que queramos dar forma la referencia a nuestro archivo scss creado al principio:

`<link rel="stylesheet" href="{{ "/assets/css/styles.css" | prepend: site.baseurl }}">`

Para proyectos grandes en los que tenemos varias hojas de estilo esta es la mejor forma de tener organizado nuestro código.
