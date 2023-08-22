 Crear un repositorio en local
•	Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
•	Crea una carpeta con el nombre del repositorio.
He creado la carpeta con el nombre Entrega-git
•	Ingresa a la carpeta que acabas de crear.
Abro Visual Studio Code y abro carpeta que he creado
•	Inicializa el repositorio de Git.
Git init
2. Subir el repositorio a GitHub
•	Crea un nuevo repositorio en GitHub.
Voy a GitHub y creo el repositorio con el mismo nombre anterior
•	Copia el URL del repositorio que acabas de crear en GitHub
Copio la URL
•	Conecta tu repositorio local con el repositorio en GitHub.
git remote add origin git@...
•	Verifica que la conexión se haya establecido correctamente.
Git remote -v
3. Hacer un commit y un push
•	Crea un archivo en la carpeta del repositorio.
Fichero1.js
•	Añade el archivo al staging.
Git add .
•	Crea un commit con un mensaje descriptivo.
Git commit -m “mi primer fichero”

•	Sube los cambios al repositorio en GitHub.
              git push --set-upstream origin master
4. Crear una rama
•	Crea una rama nueva llamada "development".
Git Branch development
•	Cambia a la nueva rama.
Git checkout development
•	Realiza algunos cambios en el archivo que creaste.
ok
•	Añade y haz un commit con los cambios en la rama "development".
Git add .
Git commit -m “cambio fichero”
•	Sube los cambios a Github.
Git push -u origin develpment
5. Hacer un merge
•	Vuelve a la rama "main".
Git checkout master
•	Haz un merge de la rama "development" a la rama "main".
Git merge development
•	Si no hay conflictos, los cambios realizados en la rama "development" se incorporarán a la rama "main".
No he tenido conflictos ya que añadí una línea mas al archivo
Si hubiera tenido conflictos habría que elegir las opciones que te da visual studio code. Y hacer un commit.
•	Haz un push de los cambios al repositorio en GitHub.
Git push