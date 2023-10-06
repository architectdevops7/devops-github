# Github Actions for CI

### Create a .github/workflows Directory:  
In your GitHub repository, create a directory named .github/workflows. This is where you'll store your workflow configuration files.  

### Create a Workflow YAML File:  
Inside the .github/workflows directory, create a YAML file (e.g., ci-cd.yml) to define your CI/CD workflow.  

**Here's an example YAML file:**  
```
name: CI/CD Pipeline

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Build
        run: |
          echo "Building..."

      - name: Test
        run: |
          echo "Testing..."

      - name: Deploy
        run: |
          echo "Deploying..."  
```
This example workflow runs on each push to the main branch and defines three jobs: build, test, and deploy.  

### Push Changes to GitHub:  
Commit and push the workflow YAML file (ci-cd.yml) to your GitHub repository.  

### GitHub Actions Execution:  
GitHub Actions will automatically detect the new workflow file and execute it when changes are pushed to the main branch.  

### Monitor and Access Logs:  
You can monitor the progress of your GitHub Actions workflows in the "Actions" tab of your GitHub repository. Detailed logs and artifacts are available for each job.  

### Configure Branch-specific Workflows:  
To create branch-specific workflows, you can modify the on section in your workflow YAML file to specify which branches should trigger the workflow.

For example, to create a workflow that runs on pushes to both main and feature branches:  
```
on:
  push:
    branches:
      - main
      - feature/*
```