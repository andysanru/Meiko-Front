# CSS

### Diseñe un arquitectura CSS (no es necesario realizar implementación en código):

```scss
$dark: #333333;

.d-flex {
    display: flex;
}

.text-dark {
    color: $dark;   
}
```
### Indique la distribución.

1. Reseteos y fuentes.
2. Cuerpo, secciones, etc.
3. Títulos, párrafos, botones, etc.
3. Clases auxiliares (Espaciado, bordes, etc).

Siempre haciendo el uso de clases y no del elemento directamente `p { //… }`-
Se mantiene un código sostenible y más limpio para el programador, y se es menos propenso a crear conflictos entre estilos.

### Qué preprocesador usaría: SASS, LESS, STYLUS, etc

**SASS**: Es uno de los más usados y en el que mejor estor adaptado-

### Comente el manejo del hack important.

La regla de estilo `!important` es utilizado con el fin de dar prioridad a un código, y se usa principalmente cuando se trabaja con platillas(Themes) ya preestablecidas o en el uso de algún framework de estilo. El uso de dicha regla se considera para algunos una mala práctica y se debe evitar siempre que se pueda en nuestros códigos.

### Incluya manejo de Themes.

El uso de themes durante un proyecto es de gran ayuda cuando un aplicativo es de bajo presupuesto y se requiere tener ciertos diseños definidos, así evitar pérdida de tiempo mayores para el programador, y su uso principalmente es porque no se tiene tiempo para crear diseños personalizado para un sitio web.
