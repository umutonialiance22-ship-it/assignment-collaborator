Working with Remotes
bash
git remote -v                        # list configured remotes
git remote add origin <url>          # link a local repo to a GitHub repo
git fetch origin                     # download remote changes without merging
git pull origin <branch>             # fetch + merge in one step
git push origin <branch>             # upload local commits
git push origin --delete <branch>    # delete a remote branch