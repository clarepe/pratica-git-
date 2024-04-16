# pratica-git-
Repositorio para prartica de comandos git 

~~~bash
git config  --global core.editor "code --wait"
~~~

O comando acima define o Visual Studio Code como o editor padrão das mensagens de commit.

~~~bash
git commit --allow-empty
~~~

O parametro `--allow-empty` permite a criação de um commit vazio, para fins de testes e pratica do Git.

~~~bash
git commit -a

~~~
O parametro `-a` adiciona todos os arquivos modificados ou não ignorados ao commit atual.

~~~bash
git checkout -b novoBranch
~~~
O parametro `-b` alterna para `novoBranch` criando o branch e indo para ele. o mesmo acontece com o comando `git switch` usando o parametro `-c`.

~~~bash
git branch -D nomebranch \\ ""apaga o branch local"
git push --delete origin nomeBranch \\ "apaga o branch do global"
~~~

para apagar um branch é preciso primeiro apaga-lo localmente (1º comando) e depois propagar a delação para repositorio remoto(2º comando)

~~~bash
git log --graph --oneline
~~~
O comando `log` exibe o historico de commits em detalhes. Com as flags `--graph` e `--oneline` exibe o historico 
em um formatomais compreencivel, atraves de um graph.
### Rebase interativo

Para alterar o autor de um commit, você pode ultilizar o rebase interativo e o comando `commit --amend`

~~~bash
git rebase -i <referencia Commit>
~~~
 ### a referencia e o commit anterior ao problema que vc quer resolver

No editor de commits, altere a instrução do commit desejado de `pick`
para `edit`. em seguida grave e feche o editor.

O rebese fará ema pausa para que você altere as informações do autor.
~~~bash
git commit --amend --reset-author --no-edit 
~~~

Caso você queira especificar o autor, ultilize a flag `--author='Nome do autor <email@autor>'`, nesse exato formato.
Caso seu commit seja vazio, acrescente ainda a flag `--allow-empty`.
Após o reparo do commit , continue o processo do rebase com o comando abaixo:
~~~bash


