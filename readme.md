#- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
`git reset --hard HEAD~1`
Use HEAD~1 para volver al commit anterior y la propiedad hard porque era 
necesario deshacer también los campos en el working copy

#- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
`git reset --hard 00eae7b`
Reset para mover el puntero HEAD y la rama al commit anterior y hard para dejar 
el working copy vacío.

#- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No. 
`Already up-to-date`

El mensaje "Ya está actualizado" aparece cuando el HEAD de la rama 
en la que se está fusionando es uno de los padres de la cadena de commits
de la rama que desea fusionar. 
No hay nada que fusionar de styled a master, ya que nada ha cambiado en master desde entonces.

#- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
Sí. Porque la rama htmilify contenía distinta versión de git-nuestro.md que styled

#- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
No. Se ha realizado de tipo fast-forward por estar en la misma cadena de commits.
HEAD ha avanzado hasta el último commit realizado. (Mergeo de styled con htmlify).

#- ¿Qué comando o comandos utilizaste en el paso 25?
`git log --graph`

#- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
Podría ser FF, no hay nuevos commits en master desde que se creo la rama title y 
se incorpora el cambio de git-nuestro.md realizado en title.
El commit realizado en title es hijo del último realizado en la rama master.

#- ¿Qué comando o comandos utilizaste en el paso 27?
`git reset HEAD~1`

#- ¿Qué comando o comandos utilizaste en el paso 28? 
`git checkout -- git-nuestro.md`

#- ¿Qué comando o comandos utilizaste en el paso 29? 
`git branch -D title`

#- ¿Qué comando o comandos utilizaste en el paso 30? 
`git reset --hard e1d223f`

#- ¿Qué comando o comandos usaste en el paso 32?
`git checkout b83a39c`

#- ¿Qué comando o comandos usaste en el punto 33?
`git checkout e1d223f`
