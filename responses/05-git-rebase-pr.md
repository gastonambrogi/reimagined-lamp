# Rebaseame mucho
El algoritmo de rebasing sirve para combinar/unificar commits en 1 solo. 
<img src="https://blog.axosoft.com/wp-content/uploads/2017/06/Squash.gif" width="400px">


Es conveniente esto al armar PR's donde la feature no necesita exponer todos los commits que necesito para su resolucion _(tenes commits que fixean cosas que antes en el mismo branch)_.

También es util para limpiar el branch y ayudar la legibilidad del log de Git.

## Paso 1: :books: Como funciona 
El algoritmo Git Rebase provee diferentes maneras de contemplar a los commits a combinar respecto al que quedará efectivo, los mas utiles son:
1. `squash` al combinar el commit con el anterior y mantiene el mensaje de ambos commits.
   1. <img src="https://blog.axosoft.com/wp-content/uploads/2017/06/Commits-to-be-squashed.gif" width="400px">
2. `fixup` combina el commit al anterior descartando el mensaje que originalmente tenia.


<hr>
<h3 align="center"> :robot: Si no ves la actividad debajo, recarga.</h3>