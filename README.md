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



```