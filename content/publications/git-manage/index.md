---
title: "Version Control with Git"
date: 2026-03-20
draft: false
authors:
  - me
tags:
  - git
  - version control
  - learning
categories:
  - Technology
summary: "Git basics for beginners"

featured: true
---

## What is Git and why do you need it?

**Git** is a distributed version control system. Simply put, it's a program that tracks changes in your files. It allows you to take "snapshots" of your project at different points in time and easily move between these snapshots.

## Key advantages of Git:

- **Change history**: You always know who, when, and why changed a particular line of code.

- **Safety**: All versions of the project are stored locally on each developer's machine, as well as (optionally) on a remote server. Data loss is practically impossible.

- **Branching**: The ability to work on new features in isolation without disrupting the stable version of the product.

- **Teamwork**: Multiple people can work on the same project simultaneously without overwriting each other's changes.

## Basic concepts

Before entering commands, it's important to understand the three levels of information storage in Git:

1. **Working Directory**: This is your current folder with files where you write code.

2. **Staging Area**: An intermediate zone. Here you gather the changes you want to save. It's like preparing a package before sending it.

3. **Repository**: The place where Git permanently stores all committed versions (commits).

## First steps: Basic workflow

Suppose you've just started a project or joined an existing one. Here are the main commands that make up 80% of daily work.

### 1. Initialization or cloning

If you're starting a project from scratch, create a folder and run:

```bash
git init
```
### 2. If you want to download an existing project from a server (for example, from GitHub):

```bash
git clone <repository_url>
```
### 3. Adding to the staging area

To tell Git, "These changes need to be saved," use the `add` command. You can add specific files or everything at once:

```bash
git add index.html    # add one file
git add .             # add all changed files in the folder
```
### 4. Commit
A commit is the "snapshot" of the project. It is important to accompany each commit with a meaningful message about what was done:

```bash
git commit -m "Added login form and fixed styles"
```
### 5. Branching

Branches are "isolated spaces." The main branch is traditionally called `main` or `master`. To create a new branch for a new feature:

```bash
git branch feature/new-login   # create a branch
git checkout feature/new-login # switch to it
```
### 6. Synchronizing with a remote repository
If you are working in a team, you will need to send your commits to the server (push) and fetch others' changes (pull).

```bash
git pull       # fetch fresh changes from the server
git push       # send your commits to the server
```
## Golden rules of working with Git

To make using Git beneficial, follow a few simple rules:

- **Commit often**: It is better to make 10 small commits with clear messages than one giant commit with the message "fixed everything".

- **Write clear messages**: A commit message should answer the question "Why?". For example: "Fixed bug #42: app crashes on empty search query".

- **Do not commit generated files**: Folders like `node_modules`, binary files, or cache should be added to a `.gitignore` file to avoid cluttering the repository.

- **Work with branches**: Never make changes directly to the `main` (or `master`) branch, especially on a team project. Use feature branches and then merge them via a Pull Request (or Merge Request).

## Popular hosting services

Git is a technology, but to conveniently share code with colleagues, people use web platforms:

- **GitHub**: The largest social network for developers.
- **GitLab**: Popular for corporate development, allows you to run your own server.
- **Bitbucket**: Often used in companies integrated with the Atlassian ecosystem.

## Conclusion

Git is a must-have tool for any developer. Do not be afraid to make mistakes, practice every day, and within a week you will feel confident!