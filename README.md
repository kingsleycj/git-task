# Task 2 - Git and Version Control
===============================================

## Version Control 

Version control, often referred to as source control, involves monitoring and managing modifications to software code. Version control systems are tools designed to assist software teams in overseeing changes to source code throughout its lifecycle.

## Difference between Git and GitHub

| **Git**                                                                                  | **GitHub**                                                                                   |
|------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| Git is a **distributed version control system** designed to track and manage changes to code locally and across teams. | GitHub is a **web-based platform** that hosts Git repositories and provides collaboration tools for developers. |
| Developers use Git locally via command-line interfaces or GUI applications to manage version control, branching, and merging. | GitHub is used online to store repositories, review code, and collaborate with team members through a graphical interface. |
| Git works offline, allowing developers to commit changes, create branches, and merge without needing internet access. Internet is only required for pushing to or pulling from remote repositories. | GitHub requires an internet connection to access repositories, collaborate, and use features like pull requests and issue tracking. |
| Git focuses solely on version control, enabling developers to track file changes, resolve conflicts, and maintain code history. | GitHub extends Git’s capabilities by providing a centralized platform for hosting repositories and offering tools for collaboration, project management, and code sharing. |
| Git is open-source software developed and maintained by the community.                   | GitHub is a proprietary platform owned by **Microsoft** since 2018.                           |

## Alternatives to GitHub

Here’s a list of three GitHub alternatives:

1. **GitLab**: An open-source platform with options for self-hosting or cloud hosting, ideal for organizations seeking a complete DevOps solution.  

2. **Bitbucket**: A repository hosting service by Atlassian, best suited for teams already using Atlassian tools like Jira.  

3. **SourceForge**: A long-established platform tailored for hosting open-source projects with community-oriented features.

## Difference between git fetch and git pull

| **Git Fetch**                                                                  | **Git Pull**                                                                  |
|-------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| **Definition**: Retrieves changes from a remote repository but does not merge them into your local branch. | **Definition**: Retrieves changes from a remote repository and merges them into your current branch. |
| **Effect on Local Branch**: Updates only the remote-tracking branches; your working branch remains unchanged. | **Effect on Local Branch**: Directly updates your working branch by incorporating the fetched changes. |
| **Use Case**: Use when you want to see what has changed on the remote without altering your local branch immediately. | **Use Case**: Use when you want to both fetch and immediately integrate remote changes into your branch. |
| **Steps Involved**: Fetches updates first; merging or rebasing must be done manually. | **Steps Involved**: Combines fetching and merging into a single command. |
| **Safety**: Safer, as it allows you to review changes before applying them. | May introduce conflicts immediately during the merge process, requiring resolution. |

## Git Rebase

**Git rebase** is a way to integrate changes from one branch into another by replaying commits from one branch onto the base of another branch. It helps to make your project history cleaner and linear by avoiding unnecessary merge commits.

### Step by Step command:
> `git checkout feature-branch`  
> `git fetch`  
> `git rebase <base>`

## Git Cherry-Pick

**Git cherry-pick** is a command that lets you apply a specific commit (or change) from one branch to another. It’s like picking a single cherry from a tree and placing it on another branch, rather than taking everything from the tree (like `git merge` or `git rebase` would do).

### Step by Step Command:

> `git checkout feature-branch`  
> `git cherry-pick <commit-hash>`
