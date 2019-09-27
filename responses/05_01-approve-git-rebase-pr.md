# Diferencia entre `git merge/git pull` y `git pull --rebase` 

## Que hace `git merge/git pull`?
Cuando actualizamos un branch con `origin`, GIT por defecto creará un merge commit involucrando los commits que combino para poder dar congruencia al log (`Merge pull request #xxx from ...`).

![Merge](https://blog.developer.atlassian.com/wp-content/uploads/2019/01/what-is-a-merge.gif)
<!-- ![Pull](http://i.imgur.com/ryRuPJS.gif) -->

## Que hace `git pull --rebase`?
Otra manera de actualizar un branch es haciendo rebase sobre un branch aplicando uno a uno los commits del branch especificado. 
De esta manera quedara en el log aplicado como si estos cambios hubieran sido efectuados en el branch que quisimos actualizar (no se crea un merge commit para esto).

![Pull Rebase](https://blog.developer.atlassian.com/wp-content/uploads/2019/01/what-is-a-rebase.gif)
<!-- ![Pull Rebase](http://i.imgur.com/o2qipCU.gif) -->

---

## Para cerrar:

### `git merge` resulta ser la opcion mas segura, agregando merge commits que no son necesarios en realidad. 
### Usar `git pull --rebase` para tener el log limpio, lineal y solo con commits que tienen cambios reales, pero requiere ser usado a conciencia.

<hr>
<h3 align="center">:robot: Para continuar, clickea en <img align="center" src="https://i.imgur.com/X3iFp1N.png" width="100px"> para mergear este PR.</h3>
