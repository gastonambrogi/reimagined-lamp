# PR desde consola ✨

**Github** creo la herramienta [HUB](https://hub.github.com/) _(desarrollado por ellos)_ para manejar Github usando la consola.
Proveen varias tareas muy utiles como manejar de issues, forkear un repo a tu cuenta personal, etc. 

En esta seccion solo vamos a usar la tarea de **Crear Pull Request's** pero podes leer mas en su documentación.

### Instalar HUB

OSX: `brew install hub`

GNU/Linux: `sudo apt-get install hub`

### Usar HUB
Para crear un PR desde el branch que estamos trabajando

1. Ejecuta `git checkout branch-cherrypicked`
2. Ejecuta `git push origin HEAD` 
   1. Necesario para `hub`
3. Ejecuta `hub pull-request --browse --base {{ user.login }}:master` 
   1. `--browse` Al terminar de crear el PR va a abrir en el Browser el PR creado.
   2. `--base` hacia que branch queremos mergear, en este caso hacia `master`
      1. `[OWNER_DEL_BRANCH]:[BRANCH_DONDE_SE_MERGEARA]`

Esto te va a abrir un editor _(VIM seguramente)_ y allí pones el contenido que tendra el PR.

EJ:

  ```shell
  Titulo del PR
  <LINEA_EN_BLANCO>
  Descripcion(opcional)
  <LINEA_EN_BLANCO>
  ---
  Ticket: https://jira.teaminspace.com/browse/JIRA-XYZ
  ```

La `<LINEA_EN_BLANCO>` _(no copies eso, simplemente deja un `Enter`)_ es necesaria para que git separe el titulo como tál y el contenido como comentario del PR.

### Documentacion

Para leer mas sobre lo que provee `hub` accede a su [documentacion](https://hub.github.com/hub.1.html).

<hr>
<h3 align="center"> :robot: Para continuar, clickea en <img align="center" src="https://i.imgur.com/K5t3DLq.png" width="100px">  para guiarte como seguir.</h3>
