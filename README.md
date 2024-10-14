# Ejercicio de Git "Libro"

## Ejercicio 1

Mostrar el historial de cambios del repositorio, a través del comando log,tanto a través de linea de comandos como modo gráfico, sigue las instrucciones del comando.

Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.

Git es un sistema de control de versiones ideado por Linus Torvalds.

Añadir los cambios a la zona de intercambio temporal(git add).

Hacer un commit de los cambios con el mensaje Añadido capítulo 1.

Volver a mostrar el historial de cambios del repositorio(git log con las opciones).

```code

 dam   main  ~  ejercicio-git-libro  git log 
commit cae8ad5fbdbd43b153bc0667a7d92a22e10864b0 (HEAD -> main, origin/main, origin/HEAD)
Author: Alexander Faustino Diaz Bautista <AlexanderFaustinoDiazBautista@Gmail.com>
Date:   Mon Oct 14 15:35:17 2024 +0100

    Initial commit
 dam   main  ~  ejercicio-git-libro  mkdir capitulos
 dam   main  ~  ejercicio-git-libro  cat > capitulos/capitulo1.txt
Git es un sistema de control de versiones ideado por Linus Torvalds.

 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Añadido capítulo 1."
[main e6ea4e5] Añadido capítulo 1.
 2 files changed, 31 insertions(+), 1 deletion(-)
 rewrite README.md (100%)
 create mode 100644 capitulos/capitulo1.txt
 dam   main  ~  ejercicio-git-libro  git log
commit e6ea4e56cd4ba7687e444bd5c289ef54a602ea83 (HEAD -> main)
Author: alexfdb <alexanderfaustinodiazbautista@gmail.com>
Date:   Mon Oct 14 15:47:46 2024 +0100

    Añadido capítulo 1.

commit cae8ad5fbdbd43b153bc0667a7d92a22e10864b0 (origin/main, origin/HEAD)
Author: Alexander Faustino Diaz Bautista <AlexanderFaustinoDiazBautista@Gmail.com>
Date:   Mon Oct 14 15:35:17 2024 +0100

    Initial commit

```

## Ejercicio 2

Crear el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto.

El flujo de trabajo básico con Git consiste en:

1- Hacer cambios en el repositorio.

2- Añadir los cambios a la zona de intercambio temporal.

3- Hacer un commit de los cambios.

Añadir los cambios a la zona de intercambio temporal.(git que comando tengo que añadir).

Hacer un commit de los cambios con el mensaje Añadido capítulo 2.

Mostrar las diferencias entre la última versión y dos versiones anteriores. (git que comando tengo que añadir).

```code

 dam   main  ~  ejercicio-git-libro  cat > capitulos/capitulo2.txt
 El flujo de trabajo básico con Git consiste en:
 1- Hacer cambios en el repositorio.
 2- Añadir los cambios a la zona de intercambio temporal.
 3- Hacer un commit de los cambios.
 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Añadido capítulo 2."
[main b1be62e] Añadido capítulo 2.
 2 files changed, 51 insertions(+)
 create mode 100644 capitulos/capitulo2.txt
 dam   main  ~  ejercicio-git-libro  git diff HEAD~2..HEAD
diff --git a/README.md b/README.md
index 9a06b52..b3f554b 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,77 @@
-# ejercicio-git-libro
\ No newline at end of file
+# Ejercicio de Git "Libro"
+
+## Ejercicio 1
+
+Mostrar el historial de cambios del repositorio, a través del comando log,tanto a través de linea de comandos como modo gráfico, sigue las instrucciones del comando.
+
+Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.
+

```

# Ejercicio 3


Crear el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto.

Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.

Añadir los cambios a la zona de intercambio temporal.

Hacer un commit de los cambios con el mensaje Añadido capítulo 3.

Mostrar las diferencias entre la primera y la última versión del repositorio.

```code

 dam   main  ~  ejercicio-git-libro  cat > capitulos/capitulo3.txt
Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.
 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Añadido capítulo 3."
[main 4c015b5] Añadido capítulo 3.
 3 files changed, 43 insertions(+), 3 deletions(-)
 create mode 100644 capitulos/capitulo3.txt
 create mode 100644 cat
 dam   main  ~  ejercicio-git-libro  git log
commit 4c015b5551c8e413df1af40011acdd777e710e4f (HEAD -> main)
Author: alexfdb <alexanderfaustinodiazbautista@gmail.com>
Date:   Mon Oct 14 16:02:11 2024 +0100

    Añadido capítulo 3.

commit b1be62e4640dd6ddce93e5b69e3e1d45c49dd7b7
Author: alexfdb <alexanderfaustinodiazbautista@gmail.com>
Date:   Mon Oct 14 15:56:55 2024 +0100

    Añadido capítulo 2.

commit e6ea4e56cd4ba7687e444bd5c289ef54a602ea83
Author: alexfdb <alexanderfaustinodiazbautista@gmail.com>
Date:   Mon Oct 14 15:47:46 2024 +0100

    Añadido capítulo 1.

commit cae8ad5fbdbd43b153bc0667a7d92a22e10864b0 (origin/main, origin/HEAD)
Author: Alexander Faustino Diaz Bautista <AlexanderFaustinoDiazBautista@Gmail.com>
Date:   Mon Oct 14 15:35:17 2024 +0100

    Initial commit
     dam   main  ~  ejercicio-git-libro  1  git diff HEAD~2..HEAD
diff --git a/README.md b/README.md
index 89a98d4..40e7466 100644
--- a/README.md
+++ b/README.md
@@ -26,5 +26,91 @@ Date:   Mon Oct 14 15:35:17 2024 +0100
  dam   main  ~  ejercicio-git-libro  cat > capitulos/capitulo1.txt
 Git es un sistema de control de versiones ideado por Linus Torvalds.
 
+ dam   main  ~  ejercicio-git-libro  git add .
+ dam   main  ~  ejercicio-git-libro  git commit -m "Añadido capítulo 1."
+[main e6ea4e5] Añadido capítulo 1.
+ 2 files changed, 31 insertions(+), 1 deletion(-)
+ rewrite README.md (100%)
+ create mode 100644 capitulos/capitulo1.txt
+ dam   main  ~  ejercicio-git-libro  git log
+commit e6ea4e56cd4ba7687e444bd5c289ef54a602ea83 (HEAD -> main)

```

# Ejercicio 4


Crea el fichero índice.txt la siguiente línea:

Indice de los cápitulos, con conceptos avanzados de git

Añadir los cambios a la zona de intercambio temporal.

Hacer un commit de los cambios con el mensaje "Indice de los cápitulos, con conceptos avanzados de git.

Mostrar quién ha hecho cambios sobre el fichero indice.txt.

```code

 dam   main  ~  ejercicio-git-libro  cat > indice.txt
 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Se crea el indice."
[main dc0efbf] Se crea el indice.
 2 files changed, 68 insertions(+)
 create mode 100644 indice.txt
 dam   main  ~  ejercicio-git-libro  echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt
 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Añadido el índice ."
[main a03772b] Añadido el índice .
 1 file changed, 1 insertion(+)
 dam   main  ~  ejercicio-git-libro  git annotate indice.txt
dc0efbfb        (   alexfdb     2024-10-14 16:14:55 +0100       1)Indice de los cápitulos, con conceptos avanzados de git
a03772b9        (   alexfdb     2024-10-14 16:15:29 +0100       2)Indice de los cápitulos, con conceptos avanzados de git

```

# Ejercicio 5

Crear una nueva rama bibliografía y mostrar las ramas del repositorio.

```code

dam   main  ~  ejercicio-git-libro  git branch bibliografia
 dam   main  ~  ejercicio-git-libro  git branch -av
  bibliografia        a03772b Añadido el índice .
* main                a03772b [adelante 5] Añadido el índice .
  remotes/origin/HEAD -> origin/main
  remotes/origin/main cae8ad5 Initial commit

```

# Ejercicio 6


Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente:

En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.

Añadir los cambios a la zona de intercambio temporal.

Hacer un commit con el mensaje “Añadido capítulo 4.”

Mostrar la historia del repositorio incluyendo todas las ramas.


```code

 dam   main  ~  ejercicio-git-libro  cat > capitulos/capitulo4.txt
En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.
 dam   main  ~  ejercicio-git-libro  git add .
 dam   main  ~  ejercicio-git-libro  git commit -m "Añadido capítulo 4."
[main 6f17f45] Añadido capítulo 4.
 3 files changed, 48 insertions(+), 3 deletions(-)
 create mode 100644 capitulos/capitulo4.txt
 dam   main  ~  ejercicio-git-libro  git log --graph --all --oneline
* 6f17f45 (HEAD -> main) Añadido capítulo 4.
* a03772b (bibliografia) Añadido el índice .
* dc0efbf Se crea el indice.
* 4c015b5 Añadido capítulo 3.
* b1be62e Añadido capítulo 2.
* e6ea4e5 Añadido capítulo 1.
* cae8ad5 (origin/main, origin/HEAD) Initial commit

```

# Ejercicio 7

Cambiar a la rama bibliografía.

Crear el fichero bibliografia.txt y añadir la siguiente referencia:

Chacon, S. and Straub, B. Pro Git. Apress.

Añadir los cambios a la zona de intercambio temporal.

Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.”

Mostrar la historia del repositorio incluyendo todas las ramas.

```code

 dam   main  ~  ejercicio-git-libro  git checkout bibliografia
Cambiado a rama 'bibliografia'
 dam   bibliografia  ~  ejercicio-git-libro  cat > bibliografia.txt
- Chacon, S. and Straub, B. Pro Git. Apress.
 dam   bibliografia  ~  ejercicio-git-libro  git add .
 dam   bibliografia  ~  ejercicio-git-libro  git commit -m "Añadida primera referencia bibliográfica."
[bibliografia 937d489] Añadida primera referencia bibliográfica.
 2 files changed, 6 insertions(+), 1 deletion(-)

```

# Ejercicio 8

Fusionar la rama bibliografía con la rama main.

Mostrar la historia del repositorio incluyendo todas las ramas.

Eliminar la rama bibliografía.

Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.

```code

 dam   main  ~  ejercicio-git-libro  git merge bibliografia
Ya está actualizado.
 dam   main  ~  ejercicio-git-libro  git log --graph --all --oneline
*   780edeb (HEAD -> main) Actualización
|\  
| * 964d7c0 (bibliografia) Actualización
| * 937d489 Añadida primera referencia bibliográfica.
* | f103fab Actualización
* | 922f84f Actualización
* | 6f17f45 Añadido capítulo 4.
|/  
* a03772b Añadido el índice .
* dc0efbf Se crea el indice.
* 4c015b5 Añadido capítulo 3.
* b1be62e Añadido capítulo 2.
* e6ea4e5 Añadido capítulo 1.
* cae8ad5 (origin/main, origin/HEAD) Initial commit
 dam   main  ~  ejercicio-git-libro  git branch -d bibliografia
Eliminada la rama bibliografia (era 964d7c0).
 dam   main  ~  ejercicio-git-libro  git log --graph --all --oneline
*   780edeb (HEAD -> main) Actualización
|\  
| * 964d7c0 Actualización
| * 937d489 Añadida primera referencia bibliográfica.
* | f103fab Actualización
* | 922f84f Actualización
* | 6f17f45 Añadido capítulo 4.
|/  
* a03772b Añadido el índice .
* dc0efbf Se crea el indice.
* 4c015b5 Añadido capítulo 3.
* b1be62e Añadido capítulo 2.
* e6ea4e5 Añadido capítulo 1.
* cae8ad5 (origin/main, origin/HEAD) Initial commit
 dam   bibliografia  ~  ejercicio-git-libro  git checkout main

 ```

 # Ejericio 9 

Crear la rama bibliografía.

Cambiar a la rama bibliografía.

Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:

Scott Chacon and Ben Straub. Pro Git. Apress.
Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014)

Cambiar a la rama main.

Cambiar el fichero bibliografia.txt para que - contenga las siguientes referencias:

Chacon, S. and Straub, B. Pro Git. Apress.

Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.

Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.”

Fusionar la rama bibliografía con la rama main.

Resolver el conflicto dejando el fichero bibliografia.txt con las referencias:

Chacon, S. and Straub, B. Pro Git. Apress.

Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.

Hodson, R. Ry’s Git Tutorial. Smashwords (2014)

Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.”

Mostrar la historia del repositorio incluyendo todas las ramas.

```code 

