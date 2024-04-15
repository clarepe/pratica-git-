# pratica-git-
Repositorio para prartica de comandos git 

~~~bash
git config  --global core.editor "code --wait"
~~~
~~~bash
git switch "e o nome do Branch" ** para trocar de branch
git  checkout "e o nome do Branch" ** para trocar de branch
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

