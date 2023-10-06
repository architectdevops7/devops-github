# Git basic commands

**git init:** Initializes a new Git repository in the current directory.  
example: **# git init**

**git clone:** Creates a copy of a remote Git repository on your local machine. It's used to download a repository for the first time.  
example: **# git clone https://github.com/user/repo.git**  

**git add:** Stages changes for commit. It tells Git which files you want to include in the next commit.  
example: **# git add filename.txt**  

**git commit:** Commits staged changes to the local repository with a descriptive message.  
example: **# git commit -m "Add a new feature"**  

**git push:** Pushes committed changes from your local repository to a remote repository, such as GitHub or GitLab.  
example: **# git push origin main**  

**git status:** Shows the current status of your working directory, including changes that are staged or not staged for commit.  
example: **# git status**  

**git log:** Displays a log of all commits in the repository, showing commit messages, authors, dates, and commit hashes.  
example: **# git log**  

**git pull:** Fetches changes from a remote repository and merges them into your local branch.  
example: **# git pull origin main**  

**git branch:** Lists all branches in the repository and highlights the current branch.  
example: **# git branch**  

**git checkout:** Switches between branches or commits, allowing you to work on different parts of your project.  
example: **# git checkout feature-branch**  

**git merge:** Combines changes from one branch into another, typically used to integrate feature branches into the main branch.  
example: **# git merge feature-branch**  

**git diff:** Shows the differences between two commits, branches, or files.  
example: **# git diff commit1 commit2**  

**git remote -v:** Lists the remote repositories that your local repository is connected to and shows their URLs.  
example: **# git remote -v**  

**git fetch:** Downloads objects and refs from another repository, updating your remote-tracking branches.  
example: **# git fetch origin**  
