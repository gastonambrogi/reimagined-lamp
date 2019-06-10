# Git log mas práctico

`git log` permite visualizar los commits del repositorio de varias maneras, asi como filtrar bajo diferentes criterios.
En esta actividad solo vamos a ver los logs entre 2 commits.

> :robot: _Tu repo esta basado en un repo template, por lo que ciertos commits que se mencionan son reales._

### :keyboard: Actividad: Ejecutar `git log` entre 2 commits

1. Ejecuta `git log 0f43333..HEAD --oneline` para ver los commits entre HEAD y un commit previo:
   1. La opcion `--oneline` reduce la informacion de los commits solo a el titulo del mismo.

### :keyboard: Actividad 2: Contar cantidad de commits desde el log

1. Para contar los cambios aplicados entre 2 commits tenemos que ejecutar:
   1. `git log 0f43333..HEAD --oneline --no-merges | wc -l`
   2. Para quitar los commits de Merge filtramos agregandole `--no-merges`
   3. Una vez que tenemos los commits que nos interesan, contamos las lineas resultantes con `wc -l`

<hr>
<h3 align="center"> :robot: Para continuar, clickea en <img align="center" src="https://i.imgur.com/K5t3DLq.png" width="100px"> para guiarte como seguir</h3>
