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
