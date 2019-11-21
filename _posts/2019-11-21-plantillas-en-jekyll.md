---
layout: post
author: leo
---
Una gran utilidad de jekyll es la reutilización de código por medio de plantillas.
Esta herramienta nos hará mucho más fácil y rápido el desarrollo de nuestro sitio web ya que podemos escribir un html para cada sección que se nos plantee: blogs, investigaciones, posts.
Por ejemplo, aunque tengamos un número considerable de posts, tan solo tendremos que tener una plantilla para ellos.


Las plantillas funcionan gracias a la etiqueta {{ content }}, redactamos la plantilla completa, dejando un hueco para el contenido variable de cada post, publicación, etc. en el que escribimos la etiqueta content, de tal forma que cada html que utilice la plantilla, reemplazará el hueco en blanco por su contenido.

Este recurso nos facilita el cumplimiento del principio de diseño de consistencia ya que nos permitirá que nuestra web sea homogénea y mejorará la navegabilidad del usuario.

Por tanto, utilizando esta herramienta nuestros htmls no necesitarán etiqueta doctype, html, head ni body, ya que estos estarán incluidos en las plantillas, solo necesitarán un front matter indicando la plantilla a usar con la sintaxis layout: plantilla.

Otro aporte curioso que hemos descubierto es que se pueden descargar plantillas gratuitamente en internet, las cuales nos facilitan un directorio parecido al que nos genera jekyll pero con los estilos y htmls del autor. El inconveniente que conlleva es que a menudo estas plantillas pueden presentar problemas de dependencias de versiones de gemas de ruby, pero como hemos instalado previamente el gestor de gemas bundler, no es un problema.

Para hacer uso de plantillas de internet, basta con ejecutar bundle install desde la terminal, dentro de la carpeta que hayamos descargado y modificar los parámetros del archivo _config.yml a nuestra necesidad.
