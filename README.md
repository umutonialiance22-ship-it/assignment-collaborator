Undoing Changes
Command	Effect
git checkout -- <file>	Discard unstaged changes to a file
git restore <file>	Modern equivalent of the above
git reset <file>	Unstage a file (keeps the edits)
git reset --soft HEAD~1	Undo last commit, keep changes staged
git reset --hard HEAD~1	Undo last commit, discard changes entirely
git revert <commit-hash>	Create a new commit that undoes a specific past commit (safe for shared history)