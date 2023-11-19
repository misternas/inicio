
# README #
Versión BETA estable.
Por favor, haz las pruebas que quieras e infórmame tanto de si hay bugs como si consideras que se puede hacer alguna mejora.


Los requerimientos necesarios para poner en marcha la plataforma DEMOKRATIAN VOTACIONES son muy sencillos. Necesita un servidor apache con php 7.4 o superior y una base de datos mysql. Dependiendo de si tiene muchos miles de inscritos el servidor tendrá que ser más o menos potente.

Tienes más información en el wiki del GIT de descarga de la aplicación
[Wiki de demokratian]( https://bitbucket.org/csalgadow/demokratian-v4/wiki/Home)


## Donar ##

Si quieres ayudarnos a mantener el proyecto, puedes hacer una donación.
[DONAR con PAYPAL](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=LAC3ZCRAWYAU2&lc=ES&item_name=Donaci%c3%b3n%20a%20%20Demokratian%2eorg&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)
También puedes donar tu tiempo y participar en el desarrollo de DEMOKRATIAN, contacta con nosotros info@demokratian.org

### ¿Para qué es este repositorio? ###

* DEMOKRATIAN VOTACIONES, una plataforma desarrollada por [Carlos Salgado Werner](http://carlos-salgado.es) para poder implementar una forma de decisión horizontal en su organización. Todos los miembros registrados podrán votar de una forma sencilla con la seguridad de que su voto es secreto.
Permite múltiples tipos de votación, actualmente dispone de 4 tipos o formas de votación. De esta forma el administrador puede elegir entre abrir un debate, realizar una encuesta, hacer una votación con voto ponderado, o realizar una votación con recuento por VUT. Además, se puede votar presencialmente en urna y luego incluir los votos mediante interventores colegiados para su posterior recuento.
DEMOKRATIAN VOTACIONES está especialmente diseñada para que sea muy fácil de usar, tanto por el usuario final, el votante, como por los distintos niveles de administradores. De esta forma no tendrá que preocuparse más que de realizar las preguntas o añadir sus candidatos para sus votaciones.
* Puedes descargar la última versión en: (https://bitbucket.org/csalgadow/demokratian-v4/downloads/)
* Tienes información adicional en el [WIKI del repositorio](https://bitbucket.org/csalgadow/demokratian-v4/wiki/Home)
)
* Web de [demokratian.org](http://demokratian.org)


### Como configurar la aplicación ###

Para instalar la aplicación, suba todos los archivos a su servidor.
Apunte su dominio o subdominio a la carpeta public_html ( de esta forma evitamos que la carpeta private sea accesible desde la red)
Las carpetas "data" que hay tanto en public_html como en private y sus subcarpetas tienen que tener permisos de escritura para el usuario con el que corre apache. (Esta ya configurado para que Ud. no tenga que modificar nada pero si hay algún problema use; chown $USUARIO.$GRUPO y chmod 0700 para ello). SI lo desea, estas carpetas puede cambiarlas de nombre posteriormente mediante el archivo de configuración.

La aplicación tiene un sistema de instalación automático, para ello debe de ir mediante su navegador a la carpeta install (midominio.org/install)
Para realizar la instalación necesita conocer los datos de la base de datos de su servidor asi como los datos de configuración del servidor de correo.
Esa información se usa para configurar el archivo config.inc.php que está en la private/carpeta config. Si por cualquier motivo la creación automática no funcionara, o posteriormente quiere hacer una modificación que no pueda realizar mediante el panel de administración de la aplicación, siempre podrá modificar ese archivo a mano.
Es posible que, si su servidor tiene poca memoria asignada, o el tiempo de ejecución de PHP es escaso, no funcione la instalación automática, en ese caso, si no puede cambiarla, tendrá que hacer una instalación manual [instrucciones de Instalación](https://bitbucket.org/csalgadow/demokratian-v4/wiki/Instalaci%C3%B3n)

Si usa una base de datos compartida con otras aplicaciones, es muy recomendable hacer una copia de seguridad de la misma antes de proceder a la instalación. Durante la misma se pueden producir errores inesperados y perder datos. Demokratian no se responsabiliza de posibles bugs o errores que puedan generar perdida de datos.  

### Modificar el aspecto de demokratian ###

Mediante la zona de administración se pueden modificar muchas cosas del aspecto exterior, incluir un blog, etc. Para otros cambios, puede modificar el tema, para hacerlo le recomendamos que haga una copia del tema demokratian, le ponga otro nombre a la carpeta, y realice los cambios que necesite. El sistema detectará que hay una nueva carpeta con un tema nuevo y podrá seleccionarlo en su configuración.

Para futuros desarrollos esperamos poder mejorar el sistema y que se puedan realizar muchos más cambios fácilmente.

### Licencia ###

Demokratian VOTACIONES es software libre bajo licencia agpl-3.0 por tanto eres libre de usarlo con las siguientes restricciones de autoría:
* Debe de mantéese en todas las paginas la nota de licencia y autoría
* Debe de dejarse en el pie de página la autoría y el nombre del software.
* Si se realizan cambios en la programación (no cambios estéticos) deberá indicarse de forma clara y publica que se trata de una versión modificada de demokratian. Si lo desea, puede enviarnos las modificaciones y si las incluimos en el desarrollo podrá no poner esa advertencia.

### Como contribuir ###

Si quieres también puedes colaborar en su desarrollo.
* Si sabes programar en PHP y te apetece mejorar la aplicación y convertirte en contribuidor, contacta con nosotros, todas las manos para mejorar y crear nuevas opciones para DEMOKRATIAN son bienvenidas.
* La nueva versión de DEMOKRATIAN permitirá cambiar el idioma y usar otros idiomas, asi que necesitamos traductores, preferentemente de Inglés, Francés, Alemán, Italiano, Euskera, Catalán, Gallego o Esperanto.
Si te animas a participar puedes hacerlo aquí [https://poeditor.com/join/project/3kA5ce9fns]   Si quieres traducirlo a otro idioma, también será muy bien venido
* También puedes colaborar haciendo una donación que nos pueden ayudar a mantener los servidores de desarrollo o animarnos a seguir desarrollando en proyecto. [DONAR con PAYPAL](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=LAC3ZCRAWYAU2&lc=ES&item_name=Donaci%c3%b3n%20a%20%20Demokratian%2eorg&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted)


### Contactar ###

Para contactar puede hacerlo mediante el correo info@demokratian.org
Aun no tenemos equipo de contribuidores así que no podemos darle más formas de contacto.

### Contribuidores ###
* En el código:
-> Antonio Garcia (rotobator[AT]gmail.com)
