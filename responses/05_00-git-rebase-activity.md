### :keyboard: Activity: Usar el rebasing 

_Vamos a hacer rebase de los ultimos 3 commits realizados en este branch._
#### Para esto vas a necesitar ejecutar algunos pasos:

1. `git checkout first-content`
2. `git pull --rebase origin first-content`
   1. :robot: _Esto no creara un commit al actualizar el branch (Por defecto al hacer `git pull` Git arma `Merge pull request #xxx from ...`)_
3. `git log master...HEAD --oneline`
   1. :robot: _Contamos los commits que hay desde master, branch de donde se creo el branch first-content, y donde estamos actualmente. Esos 3 commits que se ven es porque estamos 3 commits delante de master_
4. `git rebase -i HEAD~3`
   1. Se deja el primero como `pick 02d5b85 Update README.md`.
      1. :robot: _Los commits que dejemos como `pick` git los considerara tal cual estan sin alterarlos._
      2. :robot: _Si dejamos todos como `pick` el rebase no tendra efecto._
      3. :robot: _Git nos da una ayuda cuando entramos en rebasing:_

        ```shell
          # Commands:
          # p, pick <commit> = use commit
          # s, squash <commit> = use commit, but meld into previous commit
          # f, fixup <commit> = like "squash", but discard this commit's log message
          # ....
        ```

   2. Reemplazar desde el segundo al ultimo `pick` por `squash`. Ej: 

      ![https://miro.medium.com/max/830/1*dPaOFpMJTb5KMyS-5mO_nA.gif](https://miro.medium.com/max/830/1*dPaOFpMJTb5KMyS-5mO_nA.gif)
   3. `:wq` para salir de VIM, o `Ctrl+x` para salir si usas Nano.
   4. Luego eliminar todo el contenido del nuevo mensaje del commit que estas armando y `Escribi un mensaje sencillo que describa la feature.`
5. `git log master...HEAD --oneline`
   1. :robot: _Deberias ver como los commits originales no estan mas en el log, sino el commit que acabamos de crear._
6. `git push origin HEAD -f`
   1. :robot: _Como el branch diverge del estado original que se encuentra en Github (porque editamos la historia del branch), es necesario pushear con `-f`_


<hr>
<h3 align="center"> :robot: Para continuar, pushea tu branch <i>first-content</i> rebaseado para guiarte como seguir</h3>