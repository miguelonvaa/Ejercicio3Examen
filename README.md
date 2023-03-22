Sincroniza tu directorio del ejercicio anterior con un repositorio sin inicializar de Github llamado EJ3_EX_ED_2022.


Crear una nueva rama “refactorizacion” y mostrar las ramas del repositorio.

git branch refactorizacion


Crear el fichero refactorizacion.txt y añadir el texto siguiente:
"Refactoring is a systematic process of improving code without creating new functionality that can transform a mess into clean code and simple design."

echo "Refactoring is a systematic process of improving code without creating new functionality that can transform a mess into clean code and simple design." > refactorizacion.txt


Añadir los cambios a la zona de intercambio temporal.

git add.


Hacer un commit con el mensaje “Añadido concepto de refactorizacion”

git commit -m  “Añadido concepto de refactorizacion”


Mostrar la historia del repositorio incluyendo todas las ramas.

git status


Crear la rama “patrones”.

git branch patrones


Crear el fichero patrones.txt y añadir la siguiente referencia.

echo "Los patrones de diseño (design patterns) son soluciones habituales a problemas comunes en el diseño de software." > patrones.txt


Añadir los cambios a la zona de intercambio temporal.

git add patrones.txt


Hacer un commit con el mensaje “Añadida primera definición de patrones de diseño”.

git commit -m “Añadida primera definición de patrones de diseño”


Mostrar la historia del repositorio incluyendo todas las ramas.

git status


Fusionar la rama patrones con la rama master.

git checkout main
git merge patrones


Mostrar la historia del repositorio incluyendo todas las ramas.

git status


Eliminar la rama patrones.

git branch -D patrones


Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.

git status 


Crear la rama patrones.

git branch patrones 


Cambiar a la rama patrones.

git checkout patrones


Cambiar el fichero patrones.txt para que contenga las siguientes referencias:

echo "Cada patrón es como un plano que se puede personalizar para resolver un problema de diseño particular de tu código." > patrones.txt


Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida definición 2 de patrones de diseño”

git commit -a -m “Añadida definición 2 de patrones de diseño”


Cambiar a la rama master.

git checkout main


Cambiar el fichero patrones.txt para que contenga las siguientes referencias: "Los patrones son un juego de herramientas que brindan soluciones a problemas habituales en el diseño de software. Definen un lenguaje común que ayuda a tu equipo a comunicarse con más eficiencia."

echo "Los patrones son un juego de herramientas que brindan soluciones a problemas habituales en el diseño de software. Definen un lenguaje común que ayuda a tu equipo a comunicarse con más eficiencia." > patrones.txt


Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida definición 3.”

git commit -a -m “Añadida definición 3.”


Fusionar la rama patrones con la rama master (si existe algún conflicto, resuelvo como mejor creas).

git checkout main
vim patrones.txt
git merge patrones


Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje.

git commit -a -m “Resuelto conflicto de patrones.”


Mostrar la historia del repositorio incluyendo todas las ramas.

git log
git branch
