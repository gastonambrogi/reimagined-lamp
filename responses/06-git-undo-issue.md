# Deshaciendo cambios 

Es probable que en ciertas ocaciones sea necesario deshacer los cambios hechos en el branch que estamos trabajando.
Existen diferentes escenarios que nos podemos encontrar:

---

### Deshacer cambios locales (no agregados a stage)

Para deshacer cambios que no fueron agregados al stage (no hiciste `git add`), lo podes resolver haciendo: 
##### `git checkout -- <archivo/s>`

---

### Deshacer cambios locales (agregados a stage)

Para deshacer cambios que ya fueron agregados al stage (ya hiciste `git add`), lo podes resolver haciendo: 
##### `git reset HEAD <archivo/s>`

---

### Deshacer commit (no pusheado)

Para deshacer el commit que acabas de armar (`git add . && git commit -m '...'` y que aun no pusheaste), lo podes resolver haciendo: 
##### `git reset --soft HEAD~1`

---

### Deshacer commit (pusheado)

Para deshacer el commit que armaste y acabas de pushear el branch (`git add . && git commit -m '...' && git push origin HEAD`), lo podes resolver haciendo: 
##### `git reset --hard HEAD~1`
