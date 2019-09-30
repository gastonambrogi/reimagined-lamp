# Que es el puntero `HEAD`?

Bien! Para entender como usa Git el puntero `HEAD` internamente para referenciar al branch actual vamos a ejecutar el comando `git log`.

### :keyboard: Actividad: Ejecutar `git log`

1. Al ejecutar `git log` vamos a ver algo así:
   1. `commit 51515f6 (HEAD -> master, origin/master, origin/develop, origin/HEAD)`
   2. Lo que nos esta diciendo acá es que en mi _working-copy (copia local)_ el puntero `HEAD` apunta a `master`.

<hr>

### :keyboard: Actividad 2: Ejecutar `git log` en otro branch

1. Al hacer `git checkout develop` vamos a ver que el log ahora `HEAD` apunta a `develop`
   1. `commit 51515f6 (HEAD -> develop, origin/master, origin/develop, origin/HEAD, master)`
   2. _El 4to parametro dentro de los parentesis indica de donde se origino el branch_

<hr>
<h3 align="center"> :robot: Para continuar, clickea en <img align="center" src="https://i.imgur.com/K5t3DLq.png" width="100px"> para guiarte como seguir</h3>
