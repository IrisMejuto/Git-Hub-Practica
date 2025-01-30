# Git-Hub-Practica
Práctica del módulo de Git Hub del Bootcamp de Big Data

### 1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?

- --hard -> Elimina los cambios del Working Copy 
- HEAD~1 -> Se mueve al commit anterior

```bash
git reset --hard HEAD~1
```

### 2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

- Para encontrar el hash del commit que quiero recuperar

```bash
git reflog
```

- Para restaurar al commit anterior

```bash
git reset --hard f0d2289
```
- Para comprobar si es commit correcto

```bash
git log
```

### 3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

- No hubo ningún conflicto. Fue un merge directo "Already up to date". La rama styled ya tenía todos los cambios de main antes de absorverla.

### 4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

- Si hubo conflicto porque el archivo git-nuestro.md fue modificado en la rama styled y htmlify. El conflicto se resolvió eliminando el archivo de la rama htmlify y dejando el de styled.

### 5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

- No hubo conflictos. En este caso, no habia nuevos cambios en main que pudieran causar conflicto. Por lo que se realizó un merge Fast-forward automáticamente.

### 6. ¿Qué comando o comandos utilizaste en el paso 25?

```bash
git log --graph --decorate --pretty=oneline
```

### 7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

- No podría ser fast forward, porque main no estaba exactamente en el mismo punto que title antes del merge y tenía otros cambios después de crear la rama title, lo que hace que Git tenga que crear un commit.

```bash
git checkout main
```

```bash
git merge --no-ff title -m "Merge branch 'title' to main (no fast-forward)"
```

### 8. ¿Qué comando o comandos utilizaste en el paso 27?

- Para revertir el último commit manteniendo los cambios del Working Copy

```bash
git reset --hard HEAD~1
```
- Para guardar de forma temporal los cambios sin necesidad de hacer un commit

```bash
git stash
```

### 9. ¿Qué comando o comandos utilizaste en el paso 28?


```bash
git checkout -- git-nuestro.md
```

### 10. ¿Qué comando o comandos utilizaste en el paso 29?


```bash
git branch -D title
```

### 11. ¿Qué comando o comandos utilizaste en el paso 30?

```bash
git reflog
```

```bash
git reset --hard HEAD@{2}
```

### 12. ¿Qué comando o comandos usaste en el paso 32?

```bash
git log --oneline --graph
```

```bash
git checkout 2da86f5
```


### 13. ¿Qué comando o comandos usaste en el punto 33?

```bash
git checkout main
```
