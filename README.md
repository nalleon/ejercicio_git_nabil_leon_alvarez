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

