On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	part1/
	status_log.md

nothing added to commit but untracked files present (use "git add" to track)
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	new file:   part1/notes.txt
	new file:   part1/todo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	part1/draft.md
	status_log.md

diff --git a/part1/notes.txt b/part1/notes.txt
index e69de29..6ad36e5 100644
--- a/part1/notes.txt
+++ b/part1/notes.txt
@@ -0,0 +1,3 @@
+Line 1
+Line 2
+Line 3
diff --git a/part1/notes.txt b/part1/notes.txt
index e69de29..6ad36e5 100644
--- a/part1/notes.txt
+++ b/part1/notes.txt
@@ -0,0 +1,3 @@
+Line 1
+Line 2
+Line 3
 'git commit -a' automatically gathers modified tracked files into the staging area and commits them. It does not affect new (untracked) files.

- git fetch: Only download the changes from the remote repository to your machine without modifying the working files.
- git pull: Download the information and automatically merge those changes into the current code.
