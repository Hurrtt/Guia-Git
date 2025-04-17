# Comandos basicos para trabajar con Git

**Crear o iniciar un repositorio**

`git init`

**Clonar un repositorio**

`git clone git@github.com:Hurrtt/Guia-Git.git`

*Al momento de clonar un repositorio se descargaran todos los archivos del repo a nuestra PC*

**Area de preparacion**

`git status`

*Con git status podemos ver los cambios que hay en nuestra area de trabajo, veremos los archivos que tenemos o no tenemos agregados a nuestra area de preparacion, igualmente si han hizo modificados.*

**Añadir archivos**

`git add archivo.txt`

*Para agregar archivos a nuestra area de preparacion podemos hacerlo de uno por uno o en caso de querer agregar todo lo que tenemos en nuestra area de trabajo usamos:*

`git add . `

**Confirmar cambios**

*Una vez estemos seguros de querer subir nuestros archivos que se encuentran en el area de preparacion, debemos confirmar estos cambios y subirlos a nuestro repositorio local, esto se hace realizando un commit:*

`git commit -m "Correccion de errores"`

*En estos commits usamos el argumento "-m" para añadir una breve descripcion de que estamos agregando, eliminando o modificando con este commit.*

**Subir a repositorio remoto**

*Si queremos conectarnos a nuestro repositorio en GitHub y deseamos subir nuestros archivos primero debemos configurar la conexion en caso de no haberlo echo previamente:*

`git remote add origin git@github.com:Username/Namerepo`

*posterior a la palabra origin debemos colocar nuestro enlace SSH que nos proporciona GitHub o escribirlo a mano, unicamente debemos sustituir con el username del autor del repo y seguido con el nombre del repo*

*En caso de no tener configuradas las claves SSH en tu cuenta visita la guia de configuracion: [Claves SSH](Claves_SSH.md)*

*Una vez configurado el repositorio de forma remota subiremos nuestros cambios con:*

`git push origin nombre-rama`

*Al momento de realizar nuestro git push tendremos que indicar a que rama enviaremos estos cambios, en caso de no tener mas ramas, lo enviaremos a la rama principal llamada "main" por lo general.*

*En caso de haber modificaciones realizadas desde fuera de nuestro repositorio local, actualizaremos nuestro repositorio local usando:*

`git pull origin nombre_rama`

*En el nombre de la rama colocaremos la rama de la que queremos recibir los cambios*

**Comandos utiles**

*Si queremos consultar el historial de commits usaremos:*

`git log`

*Para consultar las modificaciones que se han echo usaremos:*

`git diff`

*En caso de querer eliminar un archivo de nuestro git usaremos:*

`git rm archivo.txt`

