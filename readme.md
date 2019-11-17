# Respuestas de la practica de GIT

**Paso 11:** 
- *git reset --hard HEAD~1* "HEAD~1" me permite volver un paso hacia atras el puntero HEAD (mi ubicacion) y la opcion "--hard" permite que GIT modifique mi WorkingCopy.

**Paso 12:**
-  *git reset --hard 75070c7* En este caso al igual que en el paso anterior "--hard" me sirve para recuperar el estado del commit (y WorkingCopy) al que hago referencia (**75070c7**a32055fd221c4ae0eb06701e146137adf). He usado tambien el comando *git reflog* para poder buscar el commit al que queria volver.

**Paso 13:**
- *Already up to date*. "Styled" tiene vision sobre master en este momento por tanto ya esta actualizado.

**Paso 19:**
- Causa conflicto porque esta vez el commit donde esta ubicado "htmlify" no tiene vision sobre el commit donde esta ubicado "styled". 

**Paso 21:**
- En este caso "Master" es el antepasado de "STYLED", no crea conflicto sino que actualiza la rama directamente. No crea conflicto.

**Paso 25:**
- *git log --graph* aunque se le pueden añadir bastantes mas parametros. *Ej: --pretty=oneline*.

**Paso 26:**
- Puede ser Fast-Forward, master se moveria a donde esta title, actualizando su contenido. En este caso el commit desde el que viene master puede seguir siendo visto por el nuevo commit al que va, es su hijo.

**Paso 27:**
- He revisado a que posicion tenia que volver con el comando  *git reflog* y en este caso he utilizado el comando *git reset HEAD@{1}*.

**Paso 28:**
- Los cambios los decarto mediante *git restore git-nuestro.md*

**Paso 29:**
- *git branch -D title* con la D mayuscula.

**Paso 30:**
- Me muevo con *git checkout 509c45015ad53282f32edd8a966cc1bf43e9aa35*. He obtenido el HASH usando *git reflog*.

**Paso 32:**
- Revisando *git log* cojo el HASH del primer commit y me muevo con *git checkout 1bdfdf1*. No lo especifica pero si se trata de mover master seria *git reset --hard 1bdfdf1*

**Paso 33:**
- Revisando *git reflog* cojo el HASH que me interesa y me muevo con *git checkout 509c450*. No lo especifica pero si se trata de mover master seria *git reset --hard 509c450*
