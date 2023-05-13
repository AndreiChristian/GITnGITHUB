# Git & GitHub Learning Guide

This guide covers the basic commands and operations in Git, a powerful version control system.

## Git Basics

### Checking Git Version

- `git --version`: This command is used to display the version of Git installed on your system.

### Initializing a Git Repository

- `git init`: This command creates a new Git repository. It can be used to convert an existing, unversioned project to a Git repository, or to initialize a new empty repository.

### Adding Files to Git

- `git add <file>`: This command updates the index using the current content found in the working tree, preparing it for the next commit. Replace `<file>` with your actual file name.

### Viewing Commit History

- `git log`: This command shows the commit history in reverse chronological order. The most recent commits are displayed at the top.

## Git Branching

### Switching Branches

- `git checkout <branch-name>`: This command switches branches by updating the index, working tree, and HEAD to reflect the chosen branch. Replace `<branch-name>` with the name of the branch you want to switch to.

- `git switch <branch-name>`: This command is a modern alternative to `git checkout <branch-name>` for switching branches. Replace `<branch-name>` with the name of the branch you want to switch to.

### Creating and Switching to a New Branch

- `git checkout -b <branch-name>`: This command creates a new branch and immediately switches to it. Replace `<branch-name>` with the name of the new branch you want to create.

- `git switch -c <branch-name>`: This command is a modern alternative to `git checkout -b <branch-name>` for creating a new branch and switching to it. Replace `<branch-name>` with the name of the new branch you want to create.

## Miscellaneous Commands

### Listing Tracked Files

- `git ls-files`: This command shows information about files in the index and the working tree.

### Checking Out Files

- `git checkout -- <file>`: This command updates the `<file>` to match the version in the index or the specified tree. If no paths are given, `git checkout` will also update `HEAD` to set the specified branch as the current branch.

### Restoring Working Tree Files

- `git restore`: This command restores working tree files.

### Cleaning the Working Tree

- `git clean -df`: This command removes untracked files from the working tree. The `-d` option tells Git to remove untracked directories as well, and the `-f` (force) option makes Git perform this action even if the "clean.requireForce" configuration option is set to true.

- `git clean -dn`: This command shows what would be done by `git clean -df`. The `-n` (dry run) option makes Git only show what would be done, without actually doing it.
