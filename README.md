Resolving Merge Conflicts

When Git can't automatically reconcile two versions of the same lines, it marks the file like this:

Steps to resolve:

Run git status to see which files are conflicted.
Open each conflicted file and look for the <<<<<<<, =======, >>>>>>> markers.
Manually edit the file to keep the correct content — one version, the other, a combination, or something new entirely.
Delete the conflict markers themselves.
Stage the resolved file:
bash
   git add README.md
Commit the resolution:
bash
   git commit -m "Resolve merge conflict in README.md"
Push the final result:
bash
   git push origin main

To back out of a conflict entirely:

bash
git merge --abort

Use case: This is the core of the activity — both teammates edited the same section of the shared file on different branches. Git couldn't decide which version was "correct," so we opened the file, compared both versions side by side, combined the best of each, and committed the resolution.