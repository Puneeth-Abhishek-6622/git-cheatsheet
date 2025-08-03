# 📝 Git Cheat Sheet

A beginner-friendly guide to essential Git commands.

---

## 📦 Project Setup

### `git init`
Initializes a new Git repository in your current directory.
```bash
git init
Creates a hidden .git/ folder to start version control.

Run this once at the beginning of a project.

📂 File Status & Changes
git status
Displays the state of the working directory and staging area.

bash
Copy
Edit
git status
Shows which files are modified, staged, or untracked.

git add
Stages changes for commit.

bash
Copy
Edit
git add <filename>     # Add specific file
git add .              # Add all changes in current directory
Prepares files for the next commit.

git commit -m "message"
Records the staged changes to the repository with a message.

bash
Copy
Edit
git commit -m "Your commit message"
Each commit should have a meaningful message describing the change.

🌱 Branching
git branch
Lists all local branches.

bash
Copy
Edit
git branch
git branch <branchname>
Creates a new branch.

bash
Copy
Edit
git branch feature-x
git checkout <branchname>
Switches to the specified branch.

bash
Copy
Edit
git checkout feature-x
🔁 Merging & Restoring
git merge <branchname>
Merges the specified branch into the current branch.

bash
Copy
Edit
git merge feature-x
Make sure you're on the branch you want to merge into.

git restore <filename>
Restores a file to the last committed state (undo changes).

bash
Copy
Edit
git restore index.html
Does not affect the commit history.

🔙 Resetting Changes
git reset <filename>
Unstages a file from the staging area (but keeps changes).

bash
Copy
Edit
git reset index.html
Useful if you accidentally staged a file.

🔗 Remote Repositories
git remote -v
Lists the remote repositories connected to your project.

bash
Copy
Edit
git remote -v
Shows URL(s) for fetch and push.

🕒 Viewing History
git log
Shows the commit history for the current branch.

bash
Copy
Edit
git log
Press q to exit log view.

✅ Quick Reference Table
Command	Description
git init	Initialize a new repo
git status	Check status of working directory
git add	Stage changes
git commit -m	Commit with message
git branch	List branches
git branch <name>	Create a new branch
git checkout <name>	Switch branches
git merge <name>	Merge a branch
git restore <file>	Restore a file
git reset <file>	Unstage a file
git remote -v	Show remotes
git log	View commit history

✍️ Tips
Always git status before committing to check what’s changed.

Use meaningful commit messages.

Use branches to separate features or bug fixes.