2. Configuration

Before using Git, configure your identity and preferences.

bash
# Set your name and email (used in every commit)
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Set default branch name for new repos
git config --global init.defaultBranch main

# Set default editor
git config --global core.editor "code --wait"

# Enable colored output
git config --global color.ui auto

# View all configuration settings
git config --list

# View a specific setting
git config user.name

Use case: Run these once per machine (or per repo with --local instead of --global) so every commit is properly attributed to you.

3. Getting Started
Initialize a repository
bash
git init

Creates a new Git repository in the current directory.

Clone an existing repository
bash
git clone https://github.com/user/repo.git
git clone https://github.com/user/repo.git my-folder-name
git clone --depth 1 https://github.com/user/repo.git   # shallow clone (faster, less history)

Use case: Shallow clones are useful in CI/CD pipelines where you only need the latest snapshot, not full history.
4. initializing repository 
git init 
5. clone an existing repository :
git clone https://github.com/user/repo.git
git clone https://github.com/user/repo.git my-folder-name
git clone --depth 1 https://github.com/user/repo.git   # shallow clone (faster, less history)
6.ckeck status and shows staged,unstaged and untracked files:
git status
7.to track all the file which is untracked use this command:
git add file.txt          # stage a specific file
git add .                 # stage everything in current directory
git add -A                # stage everything in the whole repo
git add -p                # interactively stage hunks (partial file changes)
8.commit changes :
git commit -m "anything you want to be available in your github"

