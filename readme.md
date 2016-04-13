####¿Qué comando utilizaste en el paso 11? ¿Por qué?
`git reset --hard HEAD~1`

* Para deshacer **commits** debemos usar `reset`.
* Para modificar el **working-area** debemos usar `--hard`.
* Para recuperar commits anteriores en la ubicación actual debemos indicarlo con `HEAD~n`, siendo **n** el **commit** a recuperar.

####¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
`git reflog`

`git reset --hard d986d87`

* Para saber el identificador (*hash*) del commit a rehacer debemos usar `reflog`.
* Para tener en el **working-area** el contenido del **commit** rehecho, debemos usar `--hard` con el *hash*

####El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
`git merge master`

* Para que el branch **styled** absorba al branch **master**, debemos usar `merge` desde **styled**
* **No** causó ningún conflicto porque **styled** contiene los commits de **master**

####El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

* **Si**, ya que **styled** no contiene los commits de **htmlify**, en concreto el commit del paso 18.

####El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

* **No**, porque **master** y **styled** estaban en *lista* y por como **master** estaba por debajo, se hizo un **fast forward**.

####¿Qué comando o comandos utilizaste en el paso 25?

`git log --decorate --graph --pretty=oneline`

####El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

* **Si**, porque formaban una lista.

####¿Qué comando o comandos utilizaste en el paso 27?
`git reflog`

`git reset df5bb31`

* Para no perder el contenido del **working-area** utilizamos `reset` sin `--hard` y con el *hash* del **commit** al que quiero moverme.

####¿Qué comando o comandos utilizaste en el paso 28?
`git reset --hard df5bb31`

####¿Qué comando o comandos utilizaste en el paso 29?
`git reset --d title`

`git reset --D title`

####¿Qué comando o comandos utilizaste en el paso 30?
`git reflog`

`git reset e873b1b`

`git branch title`

`git checkout title`

* Siendo **e873b1b** el *hash* del **commit** de title

####¿Qué comando o comandos usaste en el paso 32?
`git reflog`

`git reset --hard cb66466`

* Siendo **cb66466** el *hash* del **commit** inicial

####¿Qué comando o comandos usaste en el punto 33?
`git reflog`

`git reset --hard e873b1b`

* Siendo **e873b1b** el *hash* del **commit** del title
