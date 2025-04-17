# Primeros pasos para iniciar un repositorio
Una vez estemos ubicamos en la carpeta que contenga nuestro proyecto iniciaremos git con el comando:
`git init`

Para poder ejecutar nuestros primeros comandos y conectarnos a nuestro repositorio en GitHub primero debemos crear nuestro primer repositorio y configurar nuestras claves SSH para la conexion:

**Guia para crear nuestro primer repositorio en GitHub:** [Primer Repo GitHub](PrimerRepo_Github.md)

**Guia para configurar claves SSH:** [Crear Claves SSH](Claves_SSH.md)

## Primeros comandos**


```git

git init

git add README.md

git commit -m "first commit"

git branch -M main

git remote add origin git@github.com:yourusarnem/nameRepositori.git

git push -u origin main
```