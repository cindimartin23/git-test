# git-test
Repositorio para pruebas de manejo de git

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-carpeta-con-archivos)
$ git checkout
Your branch is up to date with 'origin/nueva-carpeta-con-archivos'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-carpeta-con-archivos)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 933 bytes | 311.00 KiB/s, done.
From https://github.com/cindimartin23/git-test
   b74388e..54154b6  main       -> origin/main
Updating b74388e..54154b6
Fast-forward
 New/hola-3.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 New/hola-3.txt

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git branch
  1-agregado-de-un-nuevo-archivo-hola-2txt
* main
  nueva-carpeta-con-archivos

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git checkout
Your branch is up to date with 'origin/main'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git branch nueva-rama-desde-consola

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git branch
  1-agregado-de-un-nuevo-archivo-hola-2txt
* main
  nueva-carpeta-con-archivos
  nueva-rama-desde-consola

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git push
Everything up-to-date

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git branch
  1-agregado-de-un-nuevo-archivo-hola-2txt
* main
  nueva-carpeta-con-archivos
  nueva-rama-desde-consola

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git checkout nueva-rama-desde-consola
Switched to branch 'nueva-rama-desde-consola'

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git status
On branch nueva-rama-desde-consola
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        rama-consola.txt

nothing added to commit but untracked files present (use "git add" to track)

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git add rama-consola.txt

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git status
On branch nueva-rama-desde-consola
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   rama-consola.txt


CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git commit -m 'Creado archivo en rama creada por consola'
[nueva-rama-desde-consola 5c90d88] Creado archivo en rama creada por consola
 1 file changed, 1 insertion(+)
 create mode 100644 rama-consola.txt

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git push
fatal: The current branch nueva-rama-desde-consola has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin nueva-rama-desde-consola


CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git push --set-upstream origin nueva-rama-desde-consola
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 337 bytes | 168.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'nueva-rama-desde-consola' on GitHub by visiting:
remote:      https://github.com/cindimartin23/git-test/pull/new/nueva-rama-desde-consola
remote:
To https://github.com/cindimartin23/git-test.git
 * [new branch]      nueva-rama-desde-consola -> nueva-rama-desde-consola
Branch 'nueva-rama-desde-consola' set up to track remote branch 'nueva-rama-desde-consola' from 'origin'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git checkout
Your branch is up to date with 'origin/nueva-rama-desde-consola'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (nueva-rama-desde-consola)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 927 bytes | 231.00 KiB/s, done.
From https://github.com/cindimartin23/git-test
   54154b6..d892020  main       -> origin/main
Updating 54154b6..d892020
Fast-forward
 rama-consola.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 rama-consola.txt

CINDI@LENOVO-L340 MINGW64 ~/git-test (main)
