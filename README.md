# repo_exercicio01 - Nome: Marcio Rodrigues Oliveira Gomes - RA:2400871


A - config --global
B - mkdir exercicio01
c - git init
D - echo > README.md
E - echo 01 > arquivo.txt
F - git add arquivo.txt
G - git status
H - git commit add arquivo.txt
I - echo 02 > arquivo.txt
J - git diff
K - git add arquivo.txt
L - git diff
M - echo 03 > arquivo.txt
N - git diff
O - git restore --stage arquivo.txt
P - git commit add arquivo.txt
Q - git log
R - vi .gitignore
S - echo "novo conteudo" > teste.txt


Segue abaixo o código realizado no exercício 

@MarcioRodrigues142 ➜ /workspaces/codespaces-blank $ git config --global user.name "Marcio Rodrigues Oliveira Gomes"
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank $ git config --global user.email "marcio.ogomes@aluno.faculdadeimpacta.com.br"
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank $ mkdir exercicio01
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank $ cd exercicio01/
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 $ git init
Initialized empty Git repository in /workspaces/codespaces-blank/exercicio01/.git/
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cd .git/
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ ls -a
.  ..  HEAD  branches  config  description  hooks  info  objects  refs
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01/.git (main) $ cd ..
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo "INICIANDO NO GIT" > README.md
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 01 > arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add *
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   arquivo.txt

@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add arquivo.txt"
[main (root-commit) 2947c97] git add arquivo.txt
 2 files changed, 2 insertions(+)
 create mode 100644 README.md
 create mode 100644 arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add *
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt

@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore --stage arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.tx
fatal: pathspec 'arquivo.tx' did not match any files
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit arquivo.txt
hint: Waiting for your editor to close the file... 
Aborting commit due to empty commit message.
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit  arquivo.txt
hint: Waiting for your editor to close the file... 

Aborting commit due to empty commit message.
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore --stage arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit  arquivo.txt
Aborting commit due to empty commit message.
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "git add arquivo.txt"
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

no changes added to commit (use "git add" and/or "git commit -a")
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log
commit 2947c971b7b1dc7c6f4ac06680a948feec4bda3e (HEAD -> main)
Author: Marcio Rodrigues Oliveira Gomes <marcio.ogomes@aluno.faculdadeimpacta.com.br>
Date:   Wed Aug 7 11:39:49 2024 +0000

    git add arquivo.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git gitignore
git: 'gitignore' is not a git command. See 'git --help'.
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ vi .gitignore
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo "novo conteudo" > teste.txt
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat .gitignore
*.txt
:
@MarcioRodrigues142 ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 





