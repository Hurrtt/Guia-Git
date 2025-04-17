# Primeros pasos para iniciar un repositorio
Una vez estemos ubicamos en la carpeta que contenga nuestro proyecto iniciaremos git con el comando:
`git init`

Para poder ejecutar nuestros primeros comandos y conectarnos a nuestro repositorio en GitHub primero debemos crear nuestro primer repositorio y configurar nuestras claves SSH para la conexion:

**Guia para crear nuestro primer repositorio en GitHub:** [Primer Repo GitHub](PrimerRepo_Github.md)

**Guia para configurar claves SSH:** [Crear Claves SSH](Claves_SSH.md)


## Primeros comandos

Como primer paso podemos agregar nuestro archivo "README.md" en cual puedes agregar un descripcion sobre el contenido de tu repositorio:

`git add README.md`

Una vez agregado a nuestra area de preparacion seguiremos con hacer nuestro primer commit, puedes agregar un mensaje descriptivo:

`git commit -m "first commit"`

Echo este commit nos colocaremos en nuestra rama principal: 

`git branch -M main`

Ahora conectaremos nuestro repositorio local con nuestro repositorio en GitHub:

`git remote add origin git@github.com:usarname/nombredeturepositorio.git`

*El link usado en el comando es nuestro link SSH que nos proporciona GitHub al crear nuestro repositorio*

Por ultimo haremos push a nuestra rama main y se vera reflejado en nuestro repositorio en GitHub:

`git push -u origin main`
