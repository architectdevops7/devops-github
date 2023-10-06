# Git branching commands  

**Branch Creation:** In Git, a branch is a separate line of development. You can create branches to work on new features, bug fixes, or experiments without affecting the main codebase.  
example: **# git branch feature-branch**  

Branch Switching: You can switch between branches to work on different parts of your project.  
example: **# git checkout feature-branch** 

Branch Listing: To see all branches in your repository:  
example: **# git branch**    

Branch Deletion: You can delete branches that are no longer needed.  
example: **# git branch -d feature-branch**  

# Git Merging commands:  

Merging Branches: Merging combines changes from one branch into another. For example, merging a feature branch into the main branch:  
example:  **# git merge feature-branch**    

# Git Workflow Strategies#  
Feature Branch Workflow: Create a new branch for each new feature or bug fix. Merge these branches back into the main branch when complete.

**Git Flow Workflow:** This is a branching model that defines specific branch names and their purposes, such as "feature," "release," and "hotfix" branches. It provides a structured approach to project development.  

**GitHub Flow Workflow:** Similar to the Feature Branch Workflow, this approach encourages creating feature branches but simplifies the branching model. Features are merged directly into the main branch (often called "main" or "master").  

**GitLab Flow Workflow:** Like GitHub Flow, this model simplifies the branching strategy and encourages more frequent integration with the main branch. Continuous Integration (CI) and Continuous Deployment (CD) are central to this workflow.  

**Git Pull Request Workflow:** When using platforms like GitHub or GitLab, developers create pull requests to propose changes. These changes are reviewed, discussed, and merged into the main branch.  

**Git Forking Workflow:** In an open-source context, contributors fork the repository, create branches, and submit pull requests to the original repository.  

**Centralized Workflow:** In some cases, a single central repository is used, and all developers work directly on the main branch, similar to traditional version control systems.  
