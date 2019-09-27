# Cherrypicking

Habitualmente trabajamos en diferentes branches y puede que necesitemos el cambio aplicado en otro branch que aun no fue mergeado. Otro caso comun que sucede es que creamos un commit en el branch equivocado y queremos moverlo al branch correspondiente (ej: commit en `master` :sweat:).
Para copiar este commit al branch correcto, existe la tarea `git cherry-pick`. Es preciso tener el branch actual libre de cambios sin commitear para realizar esta accion.

### Cuando usarlo 

`git cherry-pick` es una herramienta muy util pero no siempre es una buena practica. Puede causar commits duplicados si no se usa correctamente.
Al usarlo recordar 'limpiar' el branch donde se encontraba previamente el commit que se copiara.

_:robot: (lo que vimos recien sobre `git reset --hard` puede serte util :nerd_face:)_

### :keyboard: Actividad: Mover el commit a un nuevo branch
_Dejando master en su estado original_

1. `git branch branch-cherrypicked master`
   1. :robot: _Va a crear el branch mencionado partiendo del branch `master`._
2. Creá un commit en el branch `master`, no importa el cambio que hagas. 
   1. :robot: **Recorda no pushear por ahora.**
3. Ejecuta `git log` y copiate el _commitSHA_ del commit que acabas de crear.
   1. :robot: _Lo vamos a usar para la actividad._
4. `git checkout branch-cherrypicked`
5. `git cherry-pick commitSHA` _(el que copiaste antes)_
6. Volvemos el branch `master` al estado que se anterior 
   1. `git checkout master`
   2. `git reset --hard HEAD~1`
   3. `git log`
   4. :robot: _Ya no deberia estar el commit que creamos recién_
7. `git checkout branch-cherrypicked`
8. `git log`
   1. :robot: _El commit se encuentra en este branch.  :sunglasses:_
9.  **No hace falta que pushees lo hiciste.**

<hr>
<h3 align="center"> :robot: Para continuar, clickea en <img align="center" src="https://i.imgur.com/K5t3DLq.png" width="100px">  para guiarte como seguir.</h3>