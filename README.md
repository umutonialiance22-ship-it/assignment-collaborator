<<<<<<< HEAD
Setup & Configuration

Before using Git, configure your identity — this information is attached to every commit you make.

bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
=======
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
>>>>>>> df8ea33 (branch2)

Check your current configuration:

bash
git config --list

Use case: Required once per machine. Without this, Git will refuse to let you commit (or will use a generic/incorrect identity), making it impossible to tell who authored which change — a problem in team commit history.

Getting Started with a Repository
Clone an existing repository
bash
git clone https://github.com/username/repo-name.git

Downloads a full copy of the repository, including its entire history, to your machine.

Initialize a new repository
bash
git init

Turns the current folder into a Git repository (used when starting a project from scratch rather than cloning one).

Use case: clone is what each teammate runs to get their own local copy of the shared repository before creating a branch.
