BRANCHING GIT AND GITHUB COMMAND 
even if base command and an advanced command 
# List branches
git branch                 # local
git branch -r              # remote
git branch -a              # all

# Create a new branch
git branch feature/login

# Switch to a branch
git checkout feature/login
git switch feature/login   # modern alternative

# Create and switch in one step
git checkout -b feature/login
git switch -c feature/login

# Rename current branch
git branch -m new-name

# Delete a branch
git branch -d feature/login    # safe delete (merged only)
git branch -D feature/login    # force delete