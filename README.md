# Ejercicios de autoevaluación de IV

## Hito 4

**Ejercicio 9** Sistemas de integración continua.

> Darse de alta en alguno. Muchos están conectados con GitHub por lo que puedes autentificarte directamente desde ahí. A través de un proceso de autorización, puedes acceder al contenido e incluso informar del resultado de los tests a GitHub.
  
Para ello me fui a [este enlace](https://travis-ci.org), pulsé registrarme desde GitHub y como ya lo había hecho anteriormente para otros repos me salió directamente:
![](img/4-1.png) 

> Activar el repositorio en el que se vaya a aplicar la integración continua. Travis permite hacerlo directamente desde tu configuración; en otros se dan de alta desde la web de GitHub.

Desde la página a la que fui redirigida automáticamente, le di al icono de `+` para añadir el repositorio al que quiero que se haga integración continua: 

![](img/4-2.png)

Busqué goFit entre ellos, y le di al botoncico 

![](img/4-3.png)

**Ejercicio 10** Configurar integración continua para nuestra aplicación usando Travis o algún otro sitio.

Añado un fichero `.travis.yml` al directorio raíz de mi directorio

![](img/4-4.png) 

- En `language` indico que es `nodeJS`
- En `node_js` indico la versión que tiene que usar. Yo uso la versión 14.13.0, por eso pongo `14`.
- En `before_install` indico lo que tiene que hacer antes de que instale la aplicación. Instalo pues `ava` y el resto de dependencias.
- En `script` ponemos la orden que queremos que corra. 

Queda finalmente:

![](img/4-5.png)

## Hito 5 
**Ejercicio 1** Darse de alta en Vercel y Firebase, y descargarse los SDKs para poder trabajar con ellos localmente.
Me voy a [la página web de Vercel](vercel.com) y me registro con Github: 

![](img/5-1.png) 

Con lo que ya tengo mi perfil creado: 

![](img/5-2.png)

Instalamos la CLI de vercel con `npm i -g vercel` 

Para darme de alta en Firebase también me voy a la página web, me logeo con la cuenta de google y a volar: 

![](img/5-3.png) 

Añadimos elEl SDK de administrador Node.js de Firebase con `npm install firebase-admin --save`

**Ejercicio 2**  Tomar alguna de las funciones de prueba de Vercel, y hacer despliegues de prueba con el mismo.

En mi dashboard de vercel, le doy a projects y una vez ahí a importar proyecto: 

![](img/5-4.png)

Instalo vercel en mi GitHub:

![](img/5-5.png) 

Et voi là: 

![](img/5-6.png)

Creo un ejemplo básico para probar si funciona: 

~~~ 
module.exports = (req, res) => {
  res.send(`Hi there!`);
};
~~~ 

Me conecto con vercel: 

![](img/5-7.png)

Y vemos que ha funcionado woohoo: 

![](img/5-7ç8.png)

**Ejercicio 3** Tomar alguna de las funciones de prueba de Netlify, y hacer despliegues de prueba con el mismo.

Me registro también con GitHub: 

![](img/5-9.png)

Y ya tengo mi página, más bonica que tó: 

![](img/5-10.png)

Instalo la CLI: 

![](img/5-11.png)

Para lanzar un ejemplo: 

![](img/5-12.png)

![](img/5-13.png)

Me logeo con Netlify, le doy autorización a la CLI, y al hacer deploy: 

![](img/5-14.png)

Y ya estaaaAAAAaaá: 

![](img/5-15.png)