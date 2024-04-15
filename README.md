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

