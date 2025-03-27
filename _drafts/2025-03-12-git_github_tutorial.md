---
layout: single
title: "[Git/Github] Version control is a developer’s time machine."
categories: quad
tag: [Git, Github]
author_profile: false
---
## Why do we need Git and Github?
When people think of developers, they often imagine someone coding frantically in a dark room, staring at a blue-lit screen. However, in reality, the most important skills for a developer are **communication and collaboration.**

So, what is the most essential tool for development collaboration? Yes, you guessed it—`Git` and `GitHub`! These tools are the backbone of modern software teamwork and project management. 

`Git` allows developers to **track, manage, and revert** code changes efficiently. Additionally, the branching feature allows team members to **develop in parallel** without interfering with each other's work.
`Git` operates locally, but with `GitHub`, it can be pushed to the internet, **allowing developers to collaborate, share code, and review contributions**

However, once you understand the `Git` command line and how `Git` and `GitHub` can operate, you’ll soon see how powerful these tools can be.

## Basic git command lines

```bash
git init
## Initializes a Git repository; only needs to be run once per project.
## Must be executed in the correct folder; otherwise, Git will track files in the wrong directory.
```

``` bash
git add <filename>
# Stages a specific file to be included in the next commit.
git add .
# Stages all modified and new files in the current directory for the next commit.
```

**Staging** in Git means preparing selected changes to be included in the next commit, like putting files into a **‘ready to save’** list before finalizing them.

```bash
git commit -m "write commit message"
## Saves the staged changes as a new version in the repository.
```

I want to have a look at my commits!

```bash
git log
## Shows your commits
```

```bash
git remote add origin <github repository address>
## Links local Git repository to a remote repository on Github.
## Assigning github repository name to origin.
## Remote repository should not have any written codes.
## Use clone <repo> when Github repository already has a code.
```

Wait, I’d like to double-check if my GitHub repository is actually named origin.

```bash
git remote -v
## origin  https://github.com/your-username/repo-name.git (fetch)
## origin  https://github.com/your-username/repo-name.git (push)
## would mean that your github repository named origin.
```

```bash
git push <remote-repository-name> <local-branch-name>
git push origin main
## Push local commits to the main branch of the remote Github repository
```

---

## I want to modify the code while keeping the default file unchanged!

Git branch enables developers to make changes without affecting the main code until they are merged.

```bash
git branch signIn
```



