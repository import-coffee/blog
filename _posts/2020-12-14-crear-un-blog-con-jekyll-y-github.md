---
title: Crear un blog con jekyll y github pages
layout: post
tags:
- tutorial
- jekyll
- github
- blog
image: jekyll.png
---

En este tutorial hablaremos de cómo hacemos en Import Coffee para tener un blog así como las herramientas, software y servicio que empleamos para ello.
## Github
Usamos [Github](https://github.com/) como servicio web para hostear tanto la [web](http://importcoffee.es) como el blog. Cabe destacar que github solo ofrece la oportunidad de soportar paginas  [webs estaticas](https://es.wikipedia.org/wiki/P%C3%A1gina_web_est%C3%A1tica).
## Jekyll y jekyll admin
Para la creación y administración del blog nos ayudamos de [Jekyll](https://jekyllrb.com/) el cual está basado en el lenguaje [ruby](https://rubyonrails.org/) y automatiza el ensamblaje de todo el contenido del blog. Además, también usamos la extensión de [Jekyll admin](https://jekyll.github.io/jekyll-admin/) para hacer más accesible a todos los miembros de la asociación la publicación y administración de esta web.

# Instalar Jekyll 
Jekyll puede ser instalado en cualquier sistema, en este [enlace](https://jekyllrb.com/docs/installation/) podrás encontrar las instrucciones necesarias para instalar Jekyll.

# Primeros pasos
Una vez ya hemos instalado Jekyll iniciaremos un nuevo proyecto llamado blog ingresando el siguiente comando:

```
jekyll new blog
```

![](/prueba/img/tutorial1-1.png)

Tras crear el nuevo proyecto, iremos a la carpeta del proyecto recién creado:

```
cd blog
```

Por último, podremos ver una pre visualización de la página ejecutando el siguiente código en el terminal:

```
bundle exec jekyll serve
```

Una vez ejecutado, nos dirigiremos a la siguiente dirección **http://127.0.0.1:4000/** dentro del navegador.

![](/prueba/img/tutorial1-2.png)

Y veremos la página web.

![](/prueba/img/tutorial1-3.png)

En el caso de que no te guste el tema predefinido de jekyll, puedes [descargarte](http://jekyllthemes.org/) temas alternativos y [open source](https://es.wikipedia.org/wiki/C%C3%B3digo_abierto).

# Jekyll admin
Jekyll admin nos permite administrar el blog así como crear posts de forma más sencilla gracias a su interfaz gráfica.

![](/prueba/img/tutorial1-4.png)

Para instalarlo, tendremos que ir a la carpeta donde está situado nuestro blog y añadir la siguiente línea al archivo "Gemfile":

```
gem 'jekyll-admin'
```

Tal y como podemos observar en la siguiente imagen:

![](/prueba/img/tutorial1-5.png)

Guardamos los cambios y ejecutamos la siguiente línea en el terminal:

```
bundle install
```

Produciendo la siguiente salida:

![](/prueba/img/tutorial1-6.png)

Tras esto, ejecutamos nuevamente la sentencia:

```
bundle exec jekyll serve
```

Y ya podremos acceder a Jekyll admin. Para ello, iremos a la dirección **http://127.0.0.1:4000/admin/** y veremos la siguiente interfaz:

![](/prueba/img/tutorial1-7.png)

En la parte de **Posts** encontraremos todo lo relacionado a las entradas del blog, permitiendo modificar o crear entradas nuevas:

![](/prueba/img/tutorial1-8.png)

Independientemente de lo que hagas, Jekyll admin nos presentara la siguiente interfaz para editar/crear las entradas:

![](/prueba/img/tutorial1-9.png)

En los próximos tutoriales hablaremos de como subir a internet nuestro blog usando [Github](https://github.com/)  de forma gratuita.
