# confe

[Paso a Paso para implementar el desarrollo en el hosting de Git Hub]
[Tools: Visual Studio Code + Git + GitHub]

## GitHub: 
1) Con la cuenta de usuario de GitHub se crea un nuevo repositorio, en nuestro caso el repositorio es: [user / repo] Rolando-ARG/confe. Dirección de enlace: https://github.com/Rolando-ARG/confe.git

2) Se clona el repositorio a una carpeta del equipo local (cliente), en la carpeta se generan un archivo README.md (en este caso la carpeta “confe”).

3) Se mueven los archivos del proyecto de la carpeta temporal de desarrollo, a la carpeta [confe] generada por la clonación desde HitHub (no debe contener ningún archivo [.git] que no sea del propio control de versión actual).

## Visual Studio Code:
4) Se crea una nueva carpeta (temporal) y se ubican los archivos del proyecto.

5) En este punto en la carpeta [confe] continente la archivo README.md (heredado de la clonación) y los archivos index.html y styles.css y la carpeta images/ (contiene las imágenes).

6) Se ejecuta: git init
// Iniciar un nuevo repositorio
// Crear la carpeta oculta .git
Reinitialized existing Git repository in C:/……/confe/.git/

7) Se ejecuta: git status –s
// Ver que archivos no han sido registrados
?? images/
?? index.html
?? styles.css

8) Se ejecuta: git add .
// Agregar todos los archivos para que esté pendiente de los cambios
PS C:\.....\confe>

9) Se ejecuta: it commit -m "primer commit"
// Crear commit (fotografía del proyecto en ese momento)
[main 68d99a0] primer commit
 17 files changed, 303 insertions(+)
 create mode 100644 images/imagenes_integrador_front.rar
 create mode 100644 images/imagenes_integrador_front/ada.jpeg
 create mode 100644 images/imagenes_integrador_front/ba1.jpg
 create mode 100644 images/imagenes_integrador_front/ba2.jpg
 create mode 100644 images/imagenes_integrador_front/ba3.jpg
 create mode 100644 images/imagenes_integrador_front/bill.jpg
 create mode 100644 images/imagenes_integrador_front/codoacodo.png
 create mode 100644 images/imagenes_integrador_front/fjords.jpg
 create mode 100644 images/imagenes_integrador_front/hawaii.jpg
 create mode 100644 images/imagenes_integrador_front/hawaii2.jpg
 create mode 100644 images/imagenes_integrador_front/hawaii3.jpg
 create mode 100644 images/imagenes_integrador_front/honolulu.jpg
 create mode 100644 images/imagenes_integrador_front/lights.jpg
 create mode 100644 images/imagenes_integrador_front/nature.jpg
 create mode 100644 images/imagenes_integrador_front/steve.jpg
 create mode 100644 index.html
 create mode 100644 styles.css

10) Se ejecuta: git pull --rebase origin main
//Cuando realizamos cambios directamente en github pero no de forma local, es esencial realizar un pull, donde descargaremos los cambios realizados para seguir trabajando normalmente.
From https://github.com/Rolando-ARG/confe
 * branch            main       -> FETCH_HEAD
Current branch main is up to date.

11) Se ejecuta: git push origin main
//Al ejecutar el comando git push estaremos subiendo todos los cambios locales al servidor remoto de github.
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 12 threads
Compressing objects: 100% (18/18), done.
Writing objects: 100% (18/18), 6.63 MiB | 2.30 MiB/s, done.
Total 18 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/Rolando-ARG/confe.git
   124841a..68d99a0  main -> main

##GitHub: 

12) Verificamos que se hayan subido los archivos en el repositorio de GitHub.

13) En Settings/ Code and automation/Pages/Sorce: generamos la url de publicación, en este trabajo es:  https://rolando-arg.github.io/confe/




