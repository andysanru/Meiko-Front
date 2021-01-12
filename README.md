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

# Ux - Ui

### Explique brevemente qué son los Mockups y para qué son usados.

Como su nombre lo indica, son diseños creados para un aplicativo, que sirven como referencia para maquetar como se verá la interfaz de usuario, a su vez ayuda al programador (principalmente front-end) a tener idea de lo que va a realizar

### Diseñe Mockups para un Login a una plataforma Web (puede realizarlos a mano alzada).

Diseño hecho con Adobe XD, Para ver [Click aquí](https://xd.adobe.com/view/627111d5-502b-49bc-ae90-a0040c5ec662-3722/grid).

### Qué aplicación usaría para implementar los Mockups y por qué. Sea breve.

Utilizaría Adobe XD dado que tiene muchas ventajas. entre ellas:

- Es gratis, y siempre se está actualizando.
- Diseños más realistas, dado que algunos solo ofrecen hacer solo bocetos.
- Es interactivo; Esto ayuda a saber cuál es el flujo del aplicativo, tanto al cliente como al programador.

# Arquitectura en Angular 6+
Diseñe una arquitectura de dos capas (no es necesario realizar implementación en código):

**App**: módulos de la aplicación

**Store**: estado de la aplicación

**R://** Básicamente se hace uso del patrón *Redux*, en angular es normal usar *NgRx* para esto.

**App**: Contendra todos los modulos de la aplicacion, para que puedan interactuar entre si deberán llamar a un acción(borrar, editar, agregar, etc), esto a su vez provocara un cambio de estado, para obtener el estado actual se hace uso del *Store*

**Store**: Almacena toda la información de la aplicación accesible en cualquier instante, este será de solo lectura.

Mas información, [aquí](https://ngrx.io/guide/store)

# Módulos en Angular 6+
Marque la respuesta correcta y justifique brevemente.

### La mejor manera de trasportar información entre Components es:

1. Comuncación directa entre Components
2. Comuncación a través de un Service
3. Comuncación a través del Store
4. Ninguna de las anteriores

**R://** A través de un *Service*, son la mejor opción para componentes que no se conocen y transmitir información a múltiples módulos al tiempo dentro del aplicativo.

### La mejor manera de controlar el acceso a Routes es:

1. Manejar Guards a varios niveles.
2. Usar Resolvers exclusivos.
3. Aplicar Lazy Loading.
4. Ninguna de las anteriores.

**R://** Usar *Guards*, estos están diseñados para ser llamados durante la navegación del consumidor, y con la correcta implementación logran ser muy potentes para dar redirección a un usuario no autorizado.

### La autenticación, en general, debe:

1. Reposar en el Angular Module.
2. Reposar en el Shared Module.
3. Reposar en un módulo exclusivo.
4. Ninguna de las anteriores

**R://** Ninguna las anteriores, este debería ser implementado en un *Service* por aparte, donde pude llevar métodos que sean relacionados con la autenticación del usuario, como obtener información de la persona loguiada, recordar contraseña, etc.

### Si se presenta un error en el proceso de autenticación, la buena práctica es:

1. Implementar un Service para vigilar los logs.
2. Implementar un Feature en el Store para vigilar los logs.
3. Implementar un Interceptor para vigilar los logs.
4. Ninguna de las anteriores

**R://** Usar *Interceptor*, como su palabra lo indica, podemos hacer uso de estos para interceptar lo que pasa por nuestro aplicativo, entre ello vigilar los errores que ocurren y dar a conocer estos de manera más legible al usuario.

# Pruebas Unitarias

### Al realizar Unit Testing, una cobertura de 100% implica:
1. Bugs al 0%
2. Clean code al 100%
3. Funcionalidad al 100%
4. Ninguna de las anteriores

**R://** Funcionalidad al 100%, dado que estos se realizan para mantener el aplicativo con un correcto funcionamiento mientras se implementas nuevas funcionalidades, pero no implica que pueda tener errors(bugs), y mucho menos saber si se hace un *Codigo limpio*

### End to End Testing implica:

1. Flujo completo del usuario a través de pantallas
2. Interacción del usuario con componentes de cada pantalla
3. Agotar escenarios de cada pantalla
4. Ninguna de las anteriores

**R://** Flujo completo, este se da desde el punto de vista del usuario, y ya no implica código interno, se enfoca principalmente en encontrar fallas en el flujo del consumidor final.
