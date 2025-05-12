# GitHub Basics: Step-by-Step Guide (Command Line)
# This guide covers the basic steps to create a local Git repository and push it to GitHub using the command line.

**Step 1: Install Git**
If you don’t have Git installed, download and install it:

**Windows: Git for Windows**

Mac: Run git --version in Terminal (if not installed, install via Homebrew or Xcode).

Linux (Debian/Ubuntu):

sh
sudo apt update && sudo apt install git
Verify installation:

sh
**git --version**
Step 2: Configure Git (One-Time Setup)
Set your username and email (used in commits):

sh
**git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"**
Check your settings:

sh
git config --list
**Step 3: Create a Local Git Repository
Create a project folder:**

sh
**mkdir my-project
cd my-project
Initialize Git:**

sh
git init
(This creates a hidden .git folder.)

Add files (e.g., README.md):

sh
echo "# My Project" >> README.md
Check repository status:

sh
git status
Stage files (add to Git tracking):

sh
git add README.md
(Or git add . to stage all files.)

Commit changes (save locally):

sh
git commit -m "Initial commit"
Step 4: Create a GitHub Repository
Go to GitHub and log in.

Click "New" (green button) to create a repository.

Enter a Repository Name (e.g., my-project).

************************
…or create a new repository on the command line
echo "# AutomationRepo" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Lakshmi-DLT/AutomationRepo.git
git push -u origin main
********************************
…or push an existing repository from the command line
git remote add origin https://github.com/Lakshmi-DLT/AutomationRepo.git
git branch -M main
git push -u origin main
Choose Public/Private (leave other settings default).

Click "Create repository".

Step 5: Connect Local Repo to GitHub
Copy the GitHub repo URL (HTTPS or SSH):

HTTPS: https://github.com/your-username/my-project.git

SSH: git@github.com:your-username/my-project.git (requires SSH setup).

Link your local repo to GitHub:

sh
git remote add origin https://github.com/your-username/my-project.git
(Replace with your URL.)

Verify remote:

sh
git remote -v
Step 6: Push to GitHub
Push your local commits to GitHub:

sh
git push -u origin main
(If using master instead of main, replace accordingly.)

First push: -u sets upstream (future pushes can use git push).

Authentication: Enter GitHub username & password (use a Personal Access Token if prompted).

Step 7: Verify on GitHub
Refresh your GitHub repository page. Your files (e.g., README.md) should appear.

Basic Git Commands Cheat Sheet
Command	Description
git init	Initialize a local repo
git add <file>	Stage a file
git commit -m "message"	Commit changes
git remote add origin <url>	Link to GitHub
git push -u origin main	Push to GitHub
git pull	Fetch and merge changes
git clone <url>	Clone a repo
Next Steps
Branching: git branch new-feature → git checkout new-feature

Pull Requests: Collaborate on GitHub.

.gitignore: Exclude files (e.g., node_modules/).
