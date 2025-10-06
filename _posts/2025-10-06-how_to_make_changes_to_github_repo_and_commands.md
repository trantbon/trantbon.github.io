---
title: How To Make Changes To GitHub Repo And Commands
layout: post
post-image: "/assets/images/blog/cacddd39-88a9-4421-9f86-02b88b3891f8.png"
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
git status                                        # Show the working directory status

git diff                                          # Show changes not yet staged

git diff --staged                                 # Show changes staged for the next commit

git log                                           # Show commit history

## 🌿 Branching & Merging
git branch                                        # List all branches

git branch <new-branch>                           # Create a new branch

git checkout <branch-name>                        # Switch to a branch

git checkout -b <new-branch>                      # Create and switch to a new branch

git merge <branch-name>                           # Merge a branch into the current 
branch

git branch -d <branch-name>                       # Delete a branch

## 🔄 Remote Repositories
git remote -v                                     # Show remote repository URLs

git fetch                                         # Download changes from remote
 without merging

git pull                                          # Fetch and merge changes from 
remote

git push                                          # Push local commits to remote

## 🧹 Undo & Reset
git reset <file>                                  # Unstage a file

git checkout -- <file>                            # Discard changes in a file

git reset --hard <commit-id>                      # Reset to a specific commit and discard all changes

## 📥 Stashing
git stash                                         # Save changes temporarily

git stash list                                    # List all stashed changes

git stash apply                                   # Reapply the most recent stash

git stash drop                                    # Delete the most recent stash


## 🏷️ Tags
git tag                                           # List all tags

git tag <tag-name>                                # Create a new tag

git push origin <tag-name>                        # Push a tag to the remote 
repository


**Making Changes to GitHub Repo**

To make changes to a GitHub repo, you start by opening your terminal. This is the place where you type commands. Make sure you're inside the folder of the project you want to work on. Once you're there, you can open the files and make any changes you want—like fixing bugs, adding new features, or updating text. After you're done editing, go back to the terminal and type *(git add .)* to tell Git that you want to include all the changes you just made. Then type git *(commit -m "your message")*—inside the quotes, write a short note about what you changed, like "fixed login bug" or "updated homepage text." This saves your changes with a label so you can remember what you did. Finally, type *(git push)* to send your changes up to GitHub so they show up in the online repo. That’s it! Your updates are now live on GitHub.

**Merging and Creating New Branches**

 Branching in Git is like making a sandbox where you can play with new ideas without messing up your main project. It’s super useful for testing features or fixing bugs safely. To create a new branch, use *(git switch -c ______)*, which makes and switches to the branch in one go. Make sure you add the name of the branch in the blank space. After making changes, you can merge it back into the main branch *(usually called master)* by first switching back with git switch master, then running git merge feature-idea. This pulls in all your updates. Everything stays tracked inside your Git repo, so you always know what’s changed and where.

# 💻 How to Make Changes in Git and Merge Like a Pro

### Step 1
Open your terminal and make sure you're in Bash.

### Step 2
Switch into the main branch to start fresh:
git switch master

### Step 3
Pull the latest version of the code so you're working with the freshest copy:
git pull

*(Only do this if the branch exists remotely — otherwise skip it.)*

### Step 4
Create and switch to a new branch where you'll make your changes:
git switch -c <new-branch-name>

### Step 5
Make whatever changes you need in your new branch — fix bugs, add features, tweak stuff.

### Step 6
Once you're happy with the changes, run:
git add .
git commit -m "your message"
git push

If this is your first time pushing the branch, you’ll probably see this message:

(fatal: The current branch <branch-name> has no upstream branch.
To push the current branch and set the remote as upstream, use:

    git push --set-upstream origin <branch-name>)

### Step 7
Copy and paste that command into Bash:
*git push --set-upstream origin <branch-name>*

### Step 8
Now head over to your GitHub repo page. You should see a green button that says:
Compare & pull request

### Step 9
Click it. Add a short title and a quick description of what you changed.

### Step 10
Hit Create pull request. That sends your changes off for review or merging.

### Step 11
When you're ready, click Merge pull request, then Confirm merge.

### Step 12
(Optional but tidy) Click Delete branch to clean up.

# 🎉 Boom — your updates are now part of the main project!


