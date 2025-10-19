# Learning Git using [Git Immersion](https://gitimmersion.com)

This repository contains my learnings of **Git Immersion**,  a hands-on tutorial designed to deepen understanding of Git fundamentals. 

You can learn more on [Git Immersion](https://gitimmersion.com).

## Lab 1 - Setting Up and Exploring Git Basics

### 👾 Project Setup
Learned how to set up this project using a **Ruby compiler**, since Git Immersion runs as a Ruby-based tutorial.  

### Learnings

- What is the use of `git status` command?

- Learned that git works with changes, not files.


- Which files are **modified**, **staged**, or **untracked**.

- Learned that we can also use separate staging in git for commiting different files at times.
separating staging and committing, we have the ability to easily fine tune what goes into each commit.

- Learned how to modify the `git log` output format using `git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short` command the output would look like this "`fa5c03c 2025-10-13 | Added a comment (HEAD -> main, origin/main) [Aravind]`".

**Example:**
```bash
git status

git log

git log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short

```
## Lab 2 - Getting Old Versions

###  Rakefile Setup
Learned how to set up Rakefile, since Git Immersion is a Ruby-based tutorial.  

### Learnings

- How to checkout or get back previous versions of snapshots?

- What is the use of `tag` command?

- How to assign `tags` to commits?

- How to revert changes that have been **Staged** using **`git reset HEAD`** command.

- How to revert changes that have been **Commited** using **`git revert HEAD`** command.

- How to remove commits from branches or remote repositories using the **`git reset --hard <tag_name>`** command.

- How to delete tags that we no longer require with **`git tag -d <tag_name>`** command.

- How to edit previous commit or amend when we forget to add anything, if there is a typo in commit message with **`git commit -amend -m "<message>"`** command.

**Example:**
```bash
git tag - used to list all tags.

git tag <tag_name> - used to assign a tag to a commit.

git tag -d <tag_name> - used to delete a tag from the list.

git reset HEAD - used to revert changes from staging area.

git revert HEAD - used to revert changes from commited.

git reset --hard <tag_name> - used to remove changes from branches.

git commit -amend -m "<message>" - used to amend any changes like typo, files to recent commit.
