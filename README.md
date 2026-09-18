Merging

Merging combines the history of one branch into another.

bash
git checkout main
git pull origin main
git merge <branch-name>
git push origin main

Two common outcomes:

Fast-forward merge — if no one else changed main, Git just moves the pointer forward. No conflict.
Merge conflict — if both branches edited the same lines, Git stops and asks you to resolve it manually (see next section).

