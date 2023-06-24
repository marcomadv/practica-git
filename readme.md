# Práctica del curso de Git y GitHub #

Para Keepcoding | Prof. Alberto Casero - alberto@kasfactory.net  
  

## Ejercicio 1 ##

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

        Realizo un git reset --hard HEAD~1, por que este comando aparte de deshacer el commit anterior nos deshace los cambios en la zona working copy.

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

        Utilizo un git reflog para ver el id del ultimo commit que realizamos, el cual deshicimos, una vez obtengo el id uso el comando;
        · git reset --hard f33495b, esto me restaura todo al estado actual que teniamos antes de deshacer el commit, tanto el graph como el working copy

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

        En este caso no genera conflicto por que es un merge fast forward.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

        En este caso si genera conflicto, puesto que al ser un merge no fast forward y estar los ficheros git-nuestro modificados en cada rama nos lo genera, nos quedamos con los archivos de styled.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

        No genera conflicto por que el merge es fast forward.

- ¿Qué comando o comandos utilizaste en el paso 25?

        ·git log --graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

        Si, de hecho si a git no le fuerzo el --no-ff decide hacerlo de ese modo y no "no fast forward", es asi por que en main no hemos modificado nada y los dos estan en la misma "lista" no hay bifurcacion por lo que main pasa a estar con title.

- ¿Qué comando o comandos utilizaste en el paso 27?

        ·git reset HEAD~1, esto solo nos dehace el merge pero no nos toca working copy como un --hard.

- ¿Qué comando o comandos utilizaste en el paso 28?

        ·git restore git-nuestro.md, esto deshace los cambios en working copy

- ¿Qué comando o comandos utilizaste en el paso 29?

        ·git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?

        ·git reflog para el id del commit al crear el merge, mas git reset 0aa7058

- ¿Qué comando o comandos usaste en el paso 32?

        ·git reflog + git reset --hard c84da3b (para restaurar working copy de git-nuestro)

- ¿Qué comando o comandos usaste en el punto 33?

        ·git reflog + git reset --hard baa0937 (para restaurar working copy de git-nuestro con title)

