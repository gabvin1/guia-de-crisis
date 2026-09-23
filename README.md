# guia de crisis
O objetivo é aprender a colaborar atravez do git

# anotações
luno@linf:~/cris-e-chato$ git diff
diff --git a/README.md b/README.md
index d3f91c6..a10e212 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,2 @@
 # guia de crisis
+O objetivo é aprender a colaborar atravez do git
aluno@linf:~/cris-e-chato$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
aluno@linf:~/cris-e-chato$ git add .
aluno@linf:~/cris-e-chato$ git diff --staged
diff --git a/.vscode/settings.json b/.vscode/settings.json
new file mode 100644
index 0000000..a07d7ea
--- /dev/null
+++ b/.vscode/settings.json
@@ -0,0 +1,27 @@
+{
+    "workbench.view.alwaysShowHeaderActions": true,
+    "workbench.tree.renderIndentGuides": "none",
+    "[pvs]": {
+        "editor.wordSeparators": "`~!@#$%^&*()-=+[{]}|;:'\",.<>/"
+    },
+    "files.exclude": {
+        "**/.git": true,
+        "**/.svn": true,
+        "**/.hg": true,
+        "**/.DS_Store": true,
+        "**/Thumbs.db": true,
+        "**/*.???~": true,
+        "**/.pvscontext": true,
+        "**/pvsbin": true,
+        "**/*.jprf": true,
+        "**/*.prf": true,
+        "**/orphaned-proofs.prf": true,
+        "**/*_adt.pvs": false,
+        "**/*.log": false,
+        "**/.vscode": true
+    },
+    "files.readonlyInclude": {
+        "**/*.tccs": true,
aluno@linf:~/cris-e-chato$ git diff --staged
diff --git a/.vscode/settings.json b/.vscode/settings.json
new file mode 100644
index 0000000..a07d7ea
--- /dev/null
+++ b/.vscode/settings.json
@@ -0,0 +1,27 @@
+{
+    "workbench.view.alwaysShowHeaderActions": true,
+    "workbench.tree.renderIndentGuides": "none",
+    "[pvs]": {
+        "editor.wordSeparators": "`~!@#$%^&*()-=+[{]}|;:'\",.<>/"
+    },
+    "files.exclude": {
+        "**/.git": true,
+        "**/.svn": true,
+        "**/.hg": true,
+        "**/.DS_Store": true,
+        "**/Thumbs.db": true,
+        "**/*.???~": true,
+        "**/.pvscontext": true,
+        "**/pvsbin": true,
+        "**/*.jprf": true,
+        "**/*.prf": true,
+        "**/orphaned-proofs.prf": true,
+        "**/*_adt.pvs": false,
+        "**/*.log": false,
+        "**/.vscode": true
aluno@linf:~/cris-e-chato$ git commit -m "dentre as crisis, o lucas nao resolveu uma"
[main 78b8c38] dentre as crisis, o lucas nao resolveu uma
 2 files changed, 28 insertions(+)
 create mode 100644 .vscode/settings.json
aluno@linf:~/cris-e-chato$ echo "rascunho.txt" > .gitignore
aluno@linf:~/cris-e-chato$ echo "anotacoes temporarias" > .gitignore
aluno@linf:~/cris-e-chato$ echo "anotacoes temporarias" > .rascunho.txt
aluno@linf:~/cris-e-chato$ git add .
aluno@linf:~/cris-e-chato$ git commit 
.gitignore    rascunho.txt  
aluno@linf:~/cris-e-chato$ git commit 
.gitignore    rascunho.txt  
aluno@linf:~/cris-e-chato$ git commit -m 
.gitignore    rascunho.txt  
aluno@linf:~/cris-e-chato$ git commit -m "ignorar lucas e cris"
[main 53b3ef3] ignorar lucas e cris
 2 files changed, 2 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 rascunho.txt
aluno@linf:~/cris-e-chato$ git remote add origin https://github.com/gabvin1/guia-de-crisis.git
aluno@linf:~/cris-e-chato$ git push -u origin main
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (11/11), 1.22 KiB | 1.22 MiB/s, done.
Total 11 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/gabvin1/guia-de-crisis.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
aluno@linf:~/cris-e-chato$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   .gitignore

no changes added to commit (use "git add" and/or "git commit -a")
aluno@linf:~/cris-e-chato$ git add .
aluno@linf:~/cris-e-chato$ git commit -m "a amanda ta no vinil sem nos"
[main ef2c7ac] a amanda ta no vinil sem nos
 1 file changed, 2 insertions(+), 1 deletion(-)
aluno@linf:~/cris-e-chato$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/gabvin1/guia-de-crisis.git
   53b3ef3..ef2c7ac  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
aluno@linf:~/cris-e-chato$ git rm -r --cached rascunho.txt
rm 'rascunho.txt'
aluno@linf:~/cris-e-chato$ git add .
aluno@linf:~/cris-e-chato$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    rascunho.txt

aluno@linf:~/cris-e-chato$ git commit -m "Lucas n fez o rascunho sumir de primeira"
[main 1190608] Lucas n fez o rascunho sumir de primeira
 1 file changed, 1 deletion(-)
 delete mode 100644 rascunho.txt
aluno@linf:~/cris-e-chato$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 243 bytes | 243.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/gabvin1/guia-de-crisis.git
   ef2c7ac..1190608  main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.