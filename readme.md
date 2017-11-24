# Módulo 1 - **Git**
#### David López Rguez
---
- ¿Qué comando utilizaste en el **paso 11**? ¿Por qué?

`git reset –hard HEAD~1`

Usamos el comando reeset para deshacer el último commit con la opción –hard porque no queremos conservar los cambios en el working copy.

- ¿Qué comando o comandos utilizaste en el **paso 12**? ¿Por qué?

`git reflog`

`git reset –hard da4f6cf`

Usamos el commando reflog para recuperar la referencia del commit al que queremos volver y reset para movernos hacia él.

- El merge del **paso 13**, ¿Causó algún conflicto? ¿Por qué?

No causó ningún conflicto porque la rama no tiene cambios o nuevos commits desde que se creó la rama styled.

- El merge del **paso 19**, ¿Causó algún conflicto? ¿Por qué?

Dado que la rama htmlify tenia cambios en git-nuestro.md, al igual que la rama styled, el merge causó conflicto.

- El merge del **paso 21**, ¿Causó algún conflicto? ¿Por qué?

El merge no causó ningún conflicto porque, desde que se creó la rama styled, en la rama master no se han hecho commits con modificaciones en git-nuestro.md.

- ¿Qué comando o comandos utilizaste en el **paso 25**?

`git log --graph --pretty=oneline –decorate`

```
*   ee1df856aca9d1fff2fa978fda6d91a06c618160 (HEAD -> master, tag: title) Merge branch 'title'
|\  
| * 831997f1aa33a1b077fb5eb4713230900c29399b Title added
|/  
*   838247076870aec69269182a8cd1a6660a2b19e9 Merge branch 'htmlify' into styled
|\  
| * 2b14499d14b9b53235044fa165a8a8e257f41c5a (tag: htmlify) git-nuestro.md htmlify
* | da4f6cfd47804d4ac42112456b396fe1addb28f8 (tag: styled) git-nuestro.md styled
|/  
* a527c176b1e7cd6e48d69349a24e3ab7f7138503 (tag: inicial) First commit
(END)
```
- El merge del **paso 26**, ¿Podría ser fast forward? ¿Por qué?

El merge podría ser fast forward porque desde master no se habían hecho nuevos comiits desde que se creó el branch title.

- ¿Qué comando o comandos utilizaste en el **paso 27**?

`git reset HEAD~1`

- ¿Qué comando o comandos utilizaste en le **paso 28**?

`git checkout – git-nuestro.md`

- ¿Qué comando o comandos utilizaste en el **paso 29**?

`git branch –D title`

- ¿Qué comando o comandos utilizaste en el **paso 30**?

`git reflog`

`git reset --hard ee1df85`

- ¿Qué comando o comandos utilizaste en el **paso 32**?

`git reflog`

`git reset --hard a527c17`

- ¿Qué comando o comandos utilizaste en el **paso 33**?

`git reflog`
`git reset --hard ee1df85`
