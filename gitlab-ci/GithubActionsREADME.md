# Github Actions for CI

## Create a .github/workflows Directory:  
In your GitHub repository, create a directory named .github/workflows. This is where you'll store your workflow configuration files.  

## Create a Workflow YAML File:  
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