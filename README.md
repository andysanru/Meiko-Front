# Arquitectura en Angular 6+
Diseñe una arquitectura de dos capas (no es necesario realizar implementación en código):

**App**: módulos de la aplicación
**Store**: estado de la aplicación

**R://** Básicamente se hace uso del patrón *Redux*, en angular es normal usar *NgRx* para esto.

**App**: Contendra todos los modulos de la aplicacion, para que puedan interactuar entre si deberán llamar a un acción(borrar, editar, agregar, etc), esto a su vez provocara un cambio de estado, para obtener el estado actual se hace uso del *Store*

**Store**: Almacena toda la información de la aplicación accesible en cualquier instante, este será de solo lectura.

Mas información, [aquí](https://ngrx.io/guide/store)
