# Proyecto SASS Nesting

## Descripción

Proyecto desarrollado aplicando SASS como preprocesador CSS.
Se implementaron variables, nesting, metodología BEM y modularización mediante partials.

## Tecnologías utilizadas

- HTML5
- CSS3
- SASS
- Metodología BEM


## Estructura del proyecto


scss/
├── _variables.scss
├── _card.scss
├── _form.scss
└── styles.scss


Los estilos fueron separados en módulos para mejorar la organización y mantenimiento.


## Compilación SASS

Para ejecutar el proyecto:

Instalar dependencias:


npm install


Ejecutar compilación:


npm run sass



## Implementación de Nesting

Se utilizó nesting para reflejar la estructura del HTML.

Ejemplo:


.card {

&__title {}

&__content {}

}


Esto genera selectores BEM:


.card__title
.card__content



## Validación de formularios

Se implementaron las pseudo-clases:

`:valid`

Permite mostrar estilos cuando el campo cumple las reglas HTML.


`:invalid`

Permite mostrar feedback visual cuando el usuario ingresa datos incorrectos.


Los campos utilizan atributos HTML como:

- required
- type="email"


Esto permite una validación automática sin JavaScript.


## Buenas prácticas aplicadas

- Uso de variables globales.
- Partialización de archivos SASS.
- Uso de @use para importar módulos.
- Metodología BEM.
- Nesting controlado evitando exceso de especificidad.
- Código escalable y mantenible.