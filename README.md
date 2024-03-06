# GitCommands
Useful commands for GitHub ✨ <br>
Lo primero de todo es instalar Git, para instalar git nos vamos a https://git-scm.com/
o bien si estamos en windows nos instalamos winget https://learn.microsoft.com/en-us/windows/package-manager/winget/#install-winget y luego nos instalamos Git con winget install --id Git.Git -e --source winget

Una vez instalado Git hay que tener en cuenta que únicamente funciona en terminales bash, junto con la instalación de git tienes una terminal bash pero vale cuaquiera que reconozca tu sitema. Puedes añadir gitbash a tu terminal de windows como un perfil nuevo.

## GIT
#### Primeros Pasos
Iniciar sesión (Obligatorio), para ello proporcionamos un usuario y un email
Establecemos en el equipo local el usuario y correo electronico
```sh
  git config --global user.name "YourName"
  ```
```sh
  git config --global user.email "YourEmail"
  ```
Vamos al fichero .gitconfig el cual se encuentra dentro de nuestra carpeta de usuario, ahí podemos ver tanto el usuario como el correo
#### como empezar un proyecto
```sh
  cd "directorio/principal/del/proyecto"
  ```
```sh
  git init
  ```
Se nos creará una carpeta oculta para que git tenga sus parámetros, esto indicará que este directorio representa un repositorio
```sh
  git status
  ```
Para saber que commits y cambios hay realizados y demás datos
para añadir un fichero al commit hacemos:
```sh
  git add "FileName"
  ```
o bien si queremos añadir la carpeta principal entera hacemos
```sh
  git add .
  ```
para poder hacer un commit de lo que está aceptado en el status hacemos:
```sh
  git commit -m "Enunciado del commit"
  ```
Revisamos los commits
```sh
  git log
  ```
Si realizamos un cambio sin haber hecho ningun commit y queremos volver al ultimo guardado:
```sh
  git checkout "nombre del fichero"
  ```
Si después de haber hecho varios commits queremos ver de una forma más ordenada el historial, usamos:
```sh
 git log --graph --decorate --all --oneline
  ```
vamos a crear un alias del anterior comando para simplificarlo
```sh
 git config --global alias.allcommits "log --graph --decorate --all --oneline"
  ```
Si queires que un archivo nunca esté dentro de un commit creas el archivo .gitignore
```sh
  **/TestFile
  ```
Vemos los cambios realizados 
```sh
  git diff
  ```
Queremos ir a un commit concreto
```sh
  git checkout "Hash del commit"
  ```
#### Version Checker
```sh
  git -v
  ```
#### Email Checker
  ```sh
  git config --global user.email
  ```
#### User name Checker
  ```sh
  git config --global user.name
  ```
## Cosmetics
#### Confetti
```sh
  npm install canvas-confetti -E
  ```
```sh
  confetti()
```
###### <a href="https://github.com/catdad/canvas-confetti?tab=readme-ov-file">GitHub</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="https://www.kirilv.com/canvas-confetti/">Website Example</a>

## GIT Pages
