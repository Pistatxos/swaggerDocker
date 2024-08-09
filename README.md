# Proyecto Swagger con Docker


### ¿Qué es Swagger?
Swagger es una suite de herramientas para diseñar, construir, documentar y utilizar APIs. Facilita la creación de especificaciones OpenAPI, las cuales definen cómo se estructuran las API. Swagger permite a los desarrolladores y a las organizaciones gestionar el ciclo de vida completo de una API.

![Una imagen de ejemplo Swagger:](https://tomonota.net/wp-content/uploads/2024/08/Captura-de-pantalla-2024-08-08-a-las-17.14.09.png)

### ¿Cómo probar Swagger?
Tenemos varias formas de probar Swagger y el uso es igual en todos. Lo que tienen en común es que se usan desde plantillas YAML, que más adelante veremos un ejemplo.

- A traves de su web: Swagger tiene una web llamada editor.swagger.io donde puedes probar las plantillas que crees. Este editor online te permite visualizar y validar tus especificaciones OpenAPI en tiempo real. Simplemente copia y pega tu plantilla YAML en el editor y verás una representación gráfica en la parte derecha.

- Con contenedor Docker: Tenemos la posibilidad de instalarlo con docker-compose que es la opción veremos en el post.

### Instalación de Swagger usando Docker-compose
Como ya sabremos, para estas pruebas necesitaremos tener instaldo docker y docker-compose.
La estructura del proyecto lo podemos definir de la siguiente manera:
```
|-- docker-compose.yml
|-- README.md
|-- swagger.yml
|-- /swagger
    |-- ejemplo1.yaml
    |-- ejemplo2.yaml
```
- Si queremos tener desplegable para acceder a las varias plantillas debemos de guardarlas en la carpeta /swagger.
- Si queremos tener una única plantilla nos vale con guardar la plantilla como swagger.yml en raiz.

Tenemos todo explicado en la parte del código para cargar el docker-compose.


### Plantilla Swagger
Adjunto un ejemplo de plantilla con varias configuraciones para que sea más fácil a la hora de crearla.


### Configurando en nginx y opción de añadir autentificación
En la repo de Nginx Docker: [Enlace - Nginx con Docker](https://github.com/Pistatxos/nginxDocker) tenemos ejemplos para poder establecer una contraseña de acceso. Seguro que te va bien si quieres proteger el acceso, además de poder añadir un SSL y así conectar de manera segura.

Siguiendo estos ejemplos podrás configurar y probar tus APIs utilizando Swagger y Docker-compose. Os aseguro que facilitará la gestión y documentación de tus servicios de manera más eficiente y tu trabajo resaltará!

Espero que os sirva de ayuda. 

Salu2!