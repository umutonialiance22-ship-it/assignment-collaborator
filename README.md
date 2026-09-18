# View commit history
git log
git log --oneline               # condensed view
git log --graph --oneline --all # visual branch graph
git log -p                      # show diffs per commit
git log --author="Jane"
git log --since="2 weeks ago"
git log -- path/to/file          # history of a specific file

# Show a specific commit
git show <commit-hash>

# View differences
git diff                        # unstaged changes
git diff --staged               # staged changes
git diff main..feature/login    # compare branches
git diff HEAD~3 HEAD            # compare commits

# Search commit history for a string
git log -S "functionName" --oneline

