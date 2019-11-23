# GitNuestro
Práctica del curso de git, gitHub y Sourcetree

<p>
<strong>- ¿Qué comando utilizaste en el paso 11? ¿Por qué?</strong><br />
<code>git reset --hard HEAD~1</code><br />
Porque con el comando <code>git reset HEAD~1</code> conseguimos deshacer el último commit, pero manteniendo lo que había en mi Working Copy.<br />
Al añadir "-hard" (<code>git reset -hard HEAD~1</code>) conseguimos que deshaga lo que había en nuestro Working Copy al que nos desplazamos (Modifica el working copy con el commit al que nos cambiamos).
</p>

<p>
<strong>- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?</strong><br />
<code>git reflog</code><br />
<code>git reset --hard 755908f<commit_hash></code><br />
"git reflog": Para encontrar el hash SHA del commit que acabamos de borrar ("Modifico el archivo git-nuestro.md")<br />
"git reset --hard 755908f": Nos permite recuperar el commit necesario (hard es para que modifique mi Working Copy con lo que hubiera en ese commit)
</p>

<p>
<strong>- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?</strong><br />
No. No creó ningún conflicto porque la rama styled contenía todos los commits de master y no habíamos realizado ningún cambio en las 2 ramas sobre el fichero "git-nuestro.md".
</p>

<p><strong>- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?</strong><br />
Sí se produjo un conflicto:<br />
<code> CONFLICT (content): Merge conflict in git-nuestro.md</code><br />
<code> Automatic merge failed; fix conflicts and then commit the result.</code><br />
Porque el fichero git-nuestro.md había sido modificado en las 2 ramas (nos quedamos con los cambios de la rama styled).
</p>

<p><strong>- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?</strong><br />
No. No creo conflicto porque el fichero git-nuestro.md era el mismo, ya que desde la rama styled accedemos a los commits de la rama master (El merge realizado fue Fast-forward).
</p>

<p><strong>- ¿Qué comando o comandos utilizaste en el paso 25?</strong><br />
<code>git log --graph --decorate --pretty=oneline</code><br />
para que nos muestre un grafo con los commits realizados y la info de cada commit en una línea.
</p>

<p><strong>- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?</strong><br />
Sí. Porque ambas ramas forman una lista (La rama master está absorviendo a de la rama title).
</p>

<p><strong>- ¿Qué comando o comandos utilizaste en el paso 27?</strong><br />
<code>git reset HEAD~1</code>
</p>

<p><strong>- ¿Qué comando o comandos utilizaste en el paso 28?</strong><br />
<code>git checkout -- git-nuestro.md</code>
</p>

<p><strong>- ¿Qué comando o comandos utilizaste en el paso 29?</strong><br />
<code>git branch -D title</code>
</p>

<p><strong>- ¿Qué comando o comandos utilizaste en el paso 30?</strong><br />
<code>git reflog</code><br />
<code>git reset -- hard 7672970</code><br />
(Ya que reflog nos dice el hash de ese merge: <code>7672970 HEAD@{1}: merge title: Merge made by the 'recursive' strategy.</code>)
</p>

<p><strong>- ¿Qué comando o comandos usaste en el paso 32?</strong><br />
<code>git reflog</code><br />
<code>git checkout 2ce8ee7</code><br />
(Ya que reflog nos dice el hash de ese commit: <code>2ce8ee7 HEAD@{18}: commit (initial): Creamos el archivo git-nuestro.md</code>)
</p>

<p><strong>- ¿Qué comando o comandos usaste en el punto 33?</strong><br />
<code>git reflog</code><br />
<code>git checkout 6e0e7c6</code><br />
(Ya que reflog nos dice el hash de ese commit: <code>6e0e7c6 HEAD@{6}: commit: Añado un título al archivo git-nuestro.md</code>)
</p>
