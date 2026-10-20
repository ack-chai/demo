# Git Demo — Software Engineering Laboratory

**Student Name:** Abhijna Marathe  
**SRN:** PES2UG24CS020  
**GitHub Profile:** [@ack-chai](https://github.com/ack-chai)  
**Repository:** [ack-chai/demo](https://github.com/ack-chai/demo)  

---

## Overview
This repository contains the practical demonstration of fundamental Git workflows and commands for the Software Engineering laboratory assignment based on the Git Demo cheatsheet.

## Executed Git Workflows

### 1. Configuration & Local Repository Initialization
- Inspected configuration with `git config --list`.
- Initialized local repository with `git init`.
- Created `app.py`, staged files using `git add app.py` and `git add .`.
- Committed initial state with `git commit -m "Initial commit"`.

### 2. Inspecting and Undoing
- Demonstrated uncommitted changes and tracked differences with `git diff`.
- Staged changes and verified with `git diff --staged`.
- Reverted unstaged modifications using `git restore app.py` and unstaged files using `git restore --staged app.py`.

### 3. Branching, Merging & Conflict Resolution
- Branched to `feature` using `git checkout -b feature` and made changes.
- Switched to `main` with `git checkout main` / `git switch main` and made conflicting changes.
- Executed `git merge feature`, triggering a merge conflict with conflict markers `<<<<<<<`, `=======`, `>>>>>>>`.
- Manually resolved conflict in `app.py`, staged resolution with `git add app.py`, and finalized merge commit with `git commit`.
- Cleaned up local branch with `git branch -d feature`.

### 4. Remote Operations & GitHub Integration
- Renamed branch to `main` (`git branch -M main`).
- Configured remote origin: `https://github.com/ack-chai/demo.git`.
- Pushed main branch to GitHub: `git push -u origin main`.
- Demonstrated remote branch publishing and deletion: `git push origin --delete feature`.
- Verified synchronization with `git fetch`, `git pull`, and `git clone`.

---

## Commit History Graph
```text
* 4446fd3 (HEAD -> main, origin/main) Add comprehensive README documentation
*   ef342e3 Merge branch 'feature'
|\  
| * c94b854 Feature commit
* | a0c92b3 Main commit
|/  
* 783bd86 Initial commit
```

---

## Conceptual Foundations

### 1. Version Control System (VCS)
A system that records every modification made to files over time within a project repository, allowing developers to recall specific versions later, compare changes, see who contributed what, and collaborate concurrently without overwriting each other's code.

### 2. Git vs. GitHub
- **Git:** A distributed version control system (CLI tool) that runs locally on your machine, tracking history completely offline.
- **GitHub:** A cloud-based hosting service and collaboration platform built on top of Git, providing centralized repositories, pull requests, issue tracking, continuous integration (CI/CD), and team management.

### 3. Fork
A personal copy of another user's repository created under your own GitHub account. Forking allows you to freely experiment and implement changes without affecting the original upstream repository. Once changes are tested, you can propose them back to the upstream maintainer via a Pull Request (PR).
