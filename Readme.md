📝 Git & GitHub Cheat Sheet
A comprehensive, beginner-friendly guide to the most essential Git commands. Perfect for your README.md!
🚀 Getting Started
📦 git init
Initializes a new Git repository in your current directory. This creates a hidden .git/ folder to start tracking your project's history.
# Navigate to your project folder and run:
git init


⚙️ git config
Configures your Git installation. It's crucial to set your username and email, as this information will be attached to every commit you make.
# Set your name for all repositories on this computer
git config --global user.name "Your Name"

# Set your email for all repositories on this computer
git config --global user.email "youremail@example.com"


📂 The Core Workflow
git status
Displays the state of your working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git.
git status


git add
Adds changes from the working directory to the staging area. This prepares them for the next commit.
# Add a specific file
git add <filename>

# Add all new and modified files in the current directory
git add .


git commit
Records a snapshot of the staged changes to the repository's history. Each commit has a unique ID and a descriptive message.
# Commit the staged changes with a message
git commit -m "A brief, meaningful message about the changes"


🌱 Branching & Merging
Branches allow you to work on different features or fixes in isolation without affecting the main codebase.
git branch
Lists, creates, or deletes branches.
# List all local branches
git branch

# Create a new branch
git branch <branch-name>

# Delete a branch (use with caution)
git branch -d <branch-name>


git checkout
Switches between branches or restores files.
# Switch to an existing branch
git checkout <branch-name>

# Create a new branch and switch to it immediately
git checkout -b <new-branch-name>


git merge
Merges the history of a specified branch into your current branch.
# First, switch to the branch you want to merge INTO
git checkout main

# Then, merge the other branch's changes
git merge <feature-branch-name>


🔗 Working with Remote Repositories
git clone
Creates a local copy of a remote repository.
git clone <repository-url>


git remote
Manages the set of tracked remote repositories.
# List all configured remote repositories
git remote -v

# Add a new remote repository
git remote add <name> <url>
# (e.g., git remote add origin https://github.com/user/repo.git)


git push
Uploads your committed changes from your local repository to a remote repository.
# Push changes to the 'main' branch of the 'origin' remote
git push origin main


git pull
Fetches changes from a remote repository and merges them into your current local branch.
git pull origin main


🧐 Inspecting & Undoing Changes
git log
Shows the commit history for the current branch.
# See the full commit history
git log

# See a condensed version of the log
git log --oneline


git restore
Discards changes in the working directory.
# Discard changes to a specific file
git restore <filename>


git reset
Unstages a file, but preserves its contents in the working directory.
# Unstage a file that was accidentally added
git reset <filename>


✅ Quick Reference Table
Command
Description
git init
Initializes a new local repository.
git clone <url>
Creates a local copy of a remote repository.
git status
Checks the status of your working directory.
git add <file>
Stages a file for the next commit.
git commit -m "msg"
Commits staged changes with a message.
git branch <name>
Creates a new branch.
git checkout <name>
Switches to a different branch.
git merge <name>
Merges a branch into the current one.
git push
Uploads local commits to a remote repository.
git pull
Fetches and merges changes from a remote repo.
git log
Views the commit history.
git remote -v
Lists configured remote repositories.

✨ Best Practices
Commit Often: Make small, frequent commits. It's easier to find and fix bugs.
Write Good Messages: Your commit messages should be clear and concise. The first line should be a short summary (50 chars max).
Use Branches: Never work directly on the main branch. Create a new branch for every new feature or bug fix.
Pull Before You Push: Always run git pull to get the latest changes before you git push your own. This helps avoid merge conflicts.
