# BC - Menú Iconos
BC Menú Iconos

---
# Menú
El menú esta identificado con el id **#main-menu**

Número de elementos del menú
-----
Para indicar el número de elementos del menú agregar una de las siguientes clases:

Clase | Nro de elemtos | Ancho
--- | --- | ---
.menu4 | 4 | 25%
.menu5 | 5 | 20%
.menu6 | 6 | 16.66%
.menu7 | 7 | 14%
.menu8 | 8 | 12%
.menu9 | 9 | 11.11%
.menu10 | 10 | 10%
.menu11 | 11 | 9.09%
.menu12 | 12 | 8.33%
.menu13 | 13 | 7.69%

Ej.
Menú con 5 elementos
```
<ul class="menu menu5" id="main-menu">
	<li><a class="category active" href="#" data-seccion="Centros de entretenimiento" target="_top"><span class="icon"></span><span class="text">Ver Todo</span></a></li>
	<li><a class="category" href="#" data-seccion="Estantes" target="_top"><span class="icon"></span><span class="text">Televisores</span></a></li>
	<li><a class="category" href="#" data-seccion="Muebles bar" target="_top"><span class="icon"></span><span class="text">Línea Blanca</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Tablets</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Celulares</span></a></li>
</ul>
```
Menú con 7 elementos
```
<ul class="menu menu7" id="main-menu">
	<li><a class="category active" href="#" data-seccion="Centros de entretenimiento" target="_top"><span class="icon"></span><span class="text">Ver Todo</span></a></li>
	<li><a class="category" href="#" data-seccion="Estantes" target="_top"><span class="icon"></span><span class="text">Televisores</span></a></li>
	<li><a class="category" href="#" data-seccion="Muebles bar" target="_top"><span class="icon"></span><span class="text">Línea Blanca</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Tablets</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Celulares</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Celulares</span></a></li>
	<li><a class="category" href="#" data-seccion="Zapateras, veladores y cómodas" target="_top"><span class="icon"></span><span class="text">Celulares</span></a></li>
</ul>
```

Iconos
---

Dentro del elemento `<a>` con clase "**category**"; agregar un elemento `<span>` con clase "**icon**":
```
<li>
	<a class="category active" href="#" data-seccion="Centros de entretenimiento" target="_top">
		<span class="icon"></span>
		<span class="text">Ver Todo</span>
	</a>
</li>
```

La imagen que contiene los iconos debe tener las siguientes características:

* Se debe usar una imagen en formato **PNG** transparente con el nombre **master.png**
* La imagen debe tener como alto 40px y ancho un número multiplo de 24px (48px, 72px, 96px, ...).
* El orden de los iconos en el archivo master.png debe será el que se muestre en el menú.
* En la primera fila deben estar el icono en estado inactivo y en la segunda fila el estado activo.

![BC](http://jonquel.pe/landings/2017/plantillas-bc/guia-master.png)

Para mostrar el icono sobre el texto en forma vertical, agregar la clase "**menu-vertical**" al elemento `<ul>` con id "**#main-menu**"

```
<ul class="menu menu8 menu-vertical" id="main-menu">
	...
</ul>
```

![BC](http://jonquel.pe/landings/2017/plantillas-bc/horizontal-vertical.png)


Color de fondo, textos y bordes del menú en la vista mobile
-----

Se aplica sobre el elemento nav con clase "**nav**"
Para indicar el color de fondo, texto y bordes; agregar una de las siguientes etiquetas:

Clase | Color Fondo | Color Texto | Color Bordes
--- | --- | --- | ---
.menu-black | Negro | Blanco | Blanco
.menu-white | Blanco | Negro | Negro

Ej.
Fondo Negro
```
<nav class="nav menu-black collapse-movil">
	<div class="current-category">Nombre campaña</div>
	<button id="btn-mobile"><span></span><span></span><span></span></button>
	<ul class="menu menu8" id="main-menu">
		<li>...</li>
		<li>...</li>
	</ul>
</nav>
```

Fondo Blanco
```
<nav class="nav menu-white collapse-movil">
	<div class="current-category">Nombre campaña</div>
	<button id="btn-mobile"><span></span><span></span><span></span></button>
	<ul class="menu menu8" id="main-menu">
		<li>...</li>
		<li>...</li>
	</ul>
</nav>
```


Nombre de la campaña
-----

Indicar el nombre de la campaña en el elemento con clase "**.current-category**"
```
<nav class="nav menu-black collapse-movil">
	<div class="current-category">[Nombre campaña]</div>
	<button id="btn-mobile"><span></span><span></span><span></span></button>
</nav>
```
