# DiferencaIdade

Comandos Utilizados

Aqui está a explicação resumida de cada comando para integrar diretórios locais com remoto no GitHub.

echo "# DiferencaIdade" >> README.md → Cria um arquivo README.md com o texto # DiferencaIdade (um título em Markdown).

git init → Inicializa um repositório Git na pasta atual (cria a estrutura oculta .git/).

git add README.md → Adiciona o arquivo README.md ao Staging Area (preparação para o commit).

git commit -m "first commit" → Cria um commit com as alterações adicionadas, usando a mensagem "first commit".

git branch -M main → Renomeia a branch padrão (geralmente master) para main (convenção moderna).

git remote add origin https://github.com/User/Diretório(repositório).git → Vincula o repositório local a um repositório remoto (GitHub) chamado origin.

git push -u origin main → Envia (push) os commits locais para o repositório remoto (origin), na branch main. → O -u define origin/main como upstream (rastreamento automático).

Resumo Geral: Esses comandos criam um novo projeto Git, adicionam um README.md, fazem o primeiro commit e o enviam para um repositório remoto no GitHub.


*******************************************************************************************************************************
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git status
No ramo main

No commits yet

Mudanças a serem submetidas:
  (utilize "git rm --cached <arquivo>..." para não apresentar)
	new file:   .gitignore
	new file:   .idea/.gitignore
	new file:   .idea/misc.xml
	new file:   .idea/modules.xml
	new file:   .idea/vcs.xml
	new file:   DiferencaIdade.iml
	new file:   src/DiferencaIdadeSimples.java
	new file:   src/Main.java

Changes not staged for commit:
  (utilize "git add <arquivo>..." para atualizar o que será submetido)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   src/DiferencaIdadeSimples.java

Arquivos não monitorados:
  (utilize "git add <arquivo>..." para incluir o que será submetido)
	.idea/material_theme_project_new.xml

walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ echo "# DiferencaIdade" >> README.md
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git init
Reinitialized existing Git repository in /home/walter-domiciano/development/Exercicios/DiferencaIdade/.git/
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git add README.md
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git commit -m "first commit"
[main (root-commit) bd64384] first commit
 9 files changed, 83 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 .idea/.gitignore
 create mode 100644 .idea/misc.xml
 create mode 100644 .idea/modules.xml
 create mode 100644 .idea/vcs.xml
 create mode 100644 DiferencaIdade.iml
 create mode 100644 README.md
 create mode 100644 src/DiferencaIdadeSimples.java
 create mode 100644 src/Main.java
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git branch -M main
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git remote add origin https://github.com/Walterdev1k/DiferencaIdade.git
walter-domiciano:~/development/Exercicios/DiferencaIdade(git:main)$ git push -u origin main
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 4 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (13/13), 2.14 KiB | 1.07 MiB/s, done.
Total 13 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Walterdev1k/DiferencaIdade.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
