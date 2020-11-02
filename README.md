# Ejercicios de autoevaluación de IV

## Hito 4

**Ejercicio 9** Sistemas de integración continua.

> Darse de alta en alguno. Muchos están conectados con GitHub por lo que puedes autentificarte directamente desde ahí. A través de un proceso de autorización, puedes acceder al contenido e incluso informar del resultado de los tests a GitHub.
  
Para ello me fui a [este enlace](https://travis-ci.org), pulsé registrarme desde GitHub y como ya lo había hecho anteriormente para otros repos me salió directamente:
[]!(img/4-1.png) 

> Activar el repositorio en el que se vaya a aplicar la integración continua. Travis permite hacerlo directamente desde tu configuración; en otros se dan de alta desde la web de GitHub.

Desde la página a la que fui redirigida automáticamente, le di al icono de `+` para añadir el repositorio al que quiero que se haga integración continua: 

[]!(img/4-2.png)

Busqué goFit entre ellos, y le di al botoncico 

[]!(img/4-3.png)

**Ejercicio 10** Configurar integración continua para nuestra aplicación usando Travis o algún otro sitio.

Añado un fichero `.travis.yml` al directorio raíz de mi directorio

[]!(img/4-4.png) 

- En `language` indico que es `nodeJS`
- En `node_js` indico la versión que tiene que usar. Yo uso la versión 14.13.0, por eso pongo `14`.
- En `before_install` indico lo que tiene que hacer antes de que instale la aplicación. Instalo pues `ava` y el resto de dependencias.
- En `script` ponemos la orden que queremos que corra. 

Queda finalmente:

[]!(img/4-5.png)