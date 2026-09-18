
Working with Remotes


Resolving Merge Conflicts

When Git can't automatically reconcile two versions of the same lines, it marks the file like this:

Steps to resolve:

Run git status to see which files are conflicted.
Open each conflicted file and look for the <<<<<<<, =======, >>>>>>> markers.
Manually edit the file to keep the correct content — one version, the other, a combination, or something new entirely.
Delete the conflict markers themselves.
Stage the resolved file:

bash
git remote -v                        # list configured remotes
git remote add origin <url>          # link a local repo to a GitHub repo
git fetch origin                     # download remote changes without merging
git pull origin <branch>             # fetch + merge in one step
git push origin <branch>             # upload local commits
git push origin --delete <branch>    # delete a remote branch