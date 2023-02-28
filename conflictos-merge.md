### Conflictos en el Merge ###

Los conflictos en el Merge entre la rama main y proyectos se produjeron en el archivo Readme.md
Esto se dío porque ambos archivos tenían líneas con información diferente, entonces git no puede utilizar
el merge automático ya que no sabe si las líneas de los archivos erán las correctas. 

Para poder resolver este conflicto git necesita una intervención manual por parte de un usuario que verifique
si la información de los archivos es correcta y si se desean agregar las líneas con la información del Readme.md 
de las ramas **proyectos** y **main**.

Para resolver el problema, es necesario abrir con un editor de texto el archivo en cuestión y afirmar los cambios.
Cada línea estará identificada con los caracteres <<<<<<<<, >>>>>>>> y ======== dependiendo la rama. Si se desean 
mantener los cambios agregados se borran los caracteres y se guardan. Luego en la consola de git se confirman las 
acciones con el comando **git add .** y luego se comitean con **git commint -m "mesaje con la resolución del conflicto" 
