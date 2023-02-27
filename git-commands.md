# Git commands I use all the time

<img src="Images/git.png"
     alt="Git"
     style="width: 50%" />

## What is Git?

Git is a software that can be installed locally on the system. It is a command line tool to manage different versions of the edits, made to files in a git repository.

It provides functionalities like Version Control System Source Code Management.


### Commit & Push

The following I use 99% of the time:

```
git add .

git commit -m "<message>"

git push origin main
# git push takes 2 arguments
#git push REMOTE-NAME BRANCH-NAME
```

One person team, one branch (main), and I just keep commiting messages for every change I make to my own projects.

### Other commands:

To initialize a Git in a repository(repo), you use the following:

`git init`

If you are using GitHub, pushing code to a repo that's stored online, you are for sure using a remote repo. So any copied project from GitHub you can view that origin with the following command:

`git remote -v`

This will throw thew associated GitHub repo with your project. You can also initialized your own Git repo and associate it with a GitHub repo (created online).

`git remote add origin <URL>`

When you need to change the remote repository you use the following steps:


```
git remote -v
# Verifies the new remote URL

git remote add origin <url>
# Sets the new remote

git remote set-url origin <url>
```

The most common way to copy a repository is the following:

```
git clone https://github.com/USERNAME/REPOSITORY.git
# Clones a repository to your computer
```

When you run `git clone`, the following actions occur:

1. A new folder called repo is made.
1. It is initialized as a Git repository.
1. A remote named origin is created, pointing to the URL you cloned from.
1. All of the repository's files and commits are downloaded there.
1. The default branch is checked out.


When you wanto fetch changes from a remote repository - work done by other people, you use:

```
git fetch REMOTE-NAME
# Fetches updates nmade to a remote repository
```


