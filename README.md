# 1
Crea un repositorio en tu cuenta de Github con el siguiente nombre: ejercicio_git_nombre_alumno, donde nombre_alumno debe de ser tu nombre siguiendo el patrónnombre_apellido1_apellido2. No incluyas el fichero README.md.

Realiza la clonación del frepositorio creado.

Añadir el archivo README al repositorio y realizar el primer commit.

Salida:
```code 
dam@a108pc11:~$ git clone https://github.com/nalleon/ejercicio_git_nabil_leon_alvarez
Clonando en 'ejercicio_git_nabil_leon_alvarez'...
warning: Pareces haber clonado un repositorio sin contenido.
dam@a108pc11:~$ cd ejercicio_git_nabil_leon_alvarez
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ touch README.md
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git add .
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git commit -m "Se ha añadido el README.md"
[main (commit-raíz) 5d0aa92] Se ha añadido el README.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ 
```

# 2
Crear una rama con nombre develop.

Lista las ramas actuales.

Moverse a la rama y crear el fichero: hola.html. - Añadir el siguiente contenido: Sustituye nombre_alumno por tu nombre.

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Hola </title>
</head>
<body>
<h1 align="center" >Hola soy un título </h1>
<hr>
<p> Hola soy el alumno nombre_alumno </p>
</body>
</html>
```
Moverse a la rama principal y crear el fichero adios.html > Sustituye nombre_alumno por tu nombre

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Adios </title>
</head>
<body>
<h1 align="center" >Adios soy un título </h1>
<hr>
<p> Adios soy el alumno nombre_alumno </p>
</body>
</html>
```
Crea el commit con un mensaje descriptivo.
Sube los cambios a la rama actual.

```code
am@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git branch develop
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git branch 
  develop
* main
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git checkout develop
M	README.md
Cambiado a rama 'develop'
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ cat > hola.html
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Hola </title>
</head>
<body>
<h1 align="center" >Hola soy un título </h1>
<hr>
<p> Hola soy el alumno nombre_alumno </p>
</body>
</html>
^Z             
[1]+  Detenido                cat > hola.html
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ cat > hola.html
```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Hola </title>
</head>
<body>
<h1 align="center" >Hola soy un título </h1>
<hr>
<p> Hola soy el alumno Nabila León Álvarez </p>
</body>
</html>
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git checkout main
M	README.md
Cambiado a rama 'main'
Tu rama está basada en 'origin/main', pero upstream ha desaparecido.
  (usa "git branch --unset-upstream" para arreglar)
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ cat > Adios.html
     

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
<html>
<head>
<title>Adios </title>
</head>
<body>
<h1 align="center" >Adios soy un título </h1>
<hr>
<p> Adios soy el alumno Nabil León Álvarez </p>
</body>
<hmtl>
```
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git add .
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git commit "Añadido Adios.html en la rama main."
error: ruta especificada 'Añadido Adios.html en la rama main.' no concordó con ningún archivo conocido por git
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git commit -m "Añadido Adios.html en la rama main."
[main 6c81de6] Añadido Adios.html en la rama main.
 3 files changed, 48 insertions(+)
 create mode 100644 Adios.html
 create mode 100644 hola.html
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ 
```
```
# 3
Sube los cambios a la rama actual.

Lista las ramas actuales.

Realizar la mezcla en el repositorio principal.

Sube los cambios al repositorio a tu cuenta de Github.

Muestra todos los cambios realizados.

```code
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git merge develop
Ya está actualizado.
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git branch
  develop
* main
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git push origin main
Username for 'https://github.com': nalleon
Password for 'https://nalleon@github.com': 
Enumerando objetos: 11, listo.
Contando objetos: 100% (11/11), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (9/9), listo.
Escribiendo objetos: 100% (11/11), 2.18 KiB | 2.18 MiB/s, listo.
Total 11 (delta 2), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/nalleon/ejercicio_git_nabil_leon_alvarez
 * [new branch]      main -> main
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git status
En la rama main
Tu rama está actualizada con 'origin/main'.

Cambios no rastreados para el commit:
  (usa "git add <archivo>..." para actualizar lo que será confirmado)
  (usa "git restore <archivo>..." para descartar los cambios en el directorio de trabajo)
	modificados:     README.md

sin cambios agregados al commit (usa "git add" y/o "git commit -a")
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ git log
commit 8c893006b2a0b7492bd13c5ab1f9a3c4dad51ce8 (HEAD -> main, origin/main)
Author: nalleon <nabil14716@gmail.com>
Date:   Wed Oct 18 15:01:12 2023 +0100

    Actualización del README.

commit 6c81de67710240d1e49ee0a1e5adbf648bc10fb2
Author: nalleon <nabil14716@gmail.com>
Date:   Wed Oct 18 14:57:12 2023 +0100

    Añadido Adios.html en la rama main.

commit 5d0aa92f2536915a64c16bb3a8d8337d24615a6c (develop)
Author: nalleon <nabil14716@gmail.com>
Date:   Wed Oct 18 14:50:47 2023 +0100

    Se ha añadido el README.md
dam@a108pc11:~/ejercicio_git_nabil_leon_alvarez$ 
```

# 4
Lista ahora los últimos cambios que se han producido en el repositorio, es decir, los últimos commits que han realizado en el repositorio.

Lista todos los tags(etiquetas que existan).

Crea una nueva etiqueta (tag) de nombre v.1 y sube los cambios.

Crea la feature-2 y muevete a esta.

Crea el archivo Estamos_a_punto_de_terminar.html, con el siguiente contenido:

```code

```