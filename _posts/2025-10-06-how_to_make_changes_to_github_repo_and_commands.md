---
title: How To Make Changes To GitHub Repo And Commands
layout: post
post-image: "/assets/images/blog/potential-and-kinetic-energy-diagram-vector.jpg"
description: A guide no how to use the git commands properly and how to make changes to GitHub repo!
tags:
- GitHub
- Jekyll
- 
---

**All the Git Commands Need to Know**

## 🛠️ Setup & Configuration
git config --global user.name "Your Name"         # Set your Git username

git config --global user.email "you@example.com"  # Set your Git email

git config --list                                 # Show all Git config settings

## 📁 Repository Initialization
git init                                          # Create a new Git repository

git clone <repository-url>                        # Clone a remote repository

git clone -b <branch-name> <repository-url>       # Clone a specific branch from a remote repo

## 📦 Staging & Committing
git add <file>                                    # Stage a specific file

git add .                                         # Stage all changes in the current directory

git commit -m "Your commit message"               # Commit staged changes with a message

git commit -a -m "Your commit message"            # Stage and commit all tracked files

## 🔍 Status & Differences
git status                                         # Show the working directory status

git diff                                           # Show changes not yet staged

git diff --staged                                  # Show changes staged for the next commit

git log                                            # Show commit history

## 🌿 Branching & Merging
git branch                                         # List all branches

git branch <new-branch>                            # Create a new branch

git checkout <branch-name>                         # Switch to a branch

git checkout -b <new-branch>                       # Create and switch to a new branch

git merge <branch-name>                            # Merge a branch into the current 
branch

git branch -d <branch-name>                        # Delete a branch

## 🔄 Remote Repositories
git remote -v                                      # Show remote repository URLs

git fetch                                          # Download changes from remote
 without merging

git pull                                           # Fetch and merge changes from 
remote

git push                                           # Push local commits to remote

## 🧹 Undo & Reset
git reset <file>                                   # Unstage a file

git checkout -- <file>                             # Discard changes in a file

git reset --hard <commit-id>                       # Reset to a specific commit and discard all changes

## 📥 Stashing
git stash                                          # Save changes temporarily

git stash list                                     # List all stashed changes

git stash apply                                    # Reapply the most recent stash

git stash drop                                     # Delete the most recent stash


## 🏷️ Tags
git tag                                            # List all tags

git tag <tag-name>                                 # Create a new tag

git push origin <tag-name>                         # Push a tag to the remote 
repository


**Making Changes to GitHub Repo**

To make changes to a GitHub repo, you start by opening your terminal. This is the place where you type commands. Make sure you're inside the folder of the project you want to work on. Once you're there, you can open the files and make any changes you want—like fixing bugs, adding new features, or updating text. After you're done editing, go back to the terminal and type *(git add .)* to tell Git that you want to include all the changes you just made. Then type git *(commit -m "your message")*—inside the quotes, write a short note about what you changed, like "fixed login bug" or "updated homepage text." This saves your changes with a label so you can remember what you did. Finally, type *(git push)* to send your changes up to GitHub so they show up in the online repo. That’s it! Your updates are now live on GitHub.

**Merging and Creating New Branches**
Branching in Git is like making a sandbox where you can play with new ideas without messing up your main project. It’s super useful for testing features or fixing bugs safely. To create a new branch, use *(git switch -c ______)*, which makes and switches to the branch in one go. Make sure you add the name of the branch in the blank space. After making changes, you can merge it back into the main branch **(usually called master)* by first switching back with git switch master, then running git merge feature-idea. This pulls in all your updates. Everything stays tracked inside your Git repo, so you always know what’s changed and where.
