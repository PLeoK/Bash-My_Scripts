# Bash-My_Scripts

!) GIT TERMINOLOGY:
> commits
  - Essentially a snapshots of the files that you have within a particular folder (called a repository, or repo) on your system.
  - Each commit contains the changes you’ve made to the files since the last commit, so you can easily rollback those changes (much like a Windows System Restore point).

> repository (repo)

> staging
  - After creating a Git repo, you have to tell Git which files you want to version control by staging them with the git add command.
  - Staging simply adds the files to an index that represents the files that Git can take a snapshot/commit of.

!) GIT CONFIGURATION ON CLIENT MACHINE:
> git config
  $ git config --global user.name "PLeoK"
  $ git config --global user.email "przemek.kaminski6@gmail.com"
  $ git config --list # To list your configuration 

!) TO TURN AN EXISTING FOLDER INTO A GIT REPO:
> When in the directory you want to turn in to repo:
  $ git init

!) STAGE FILE(S) FOR COMMIT:
> use "git add <file>..." to include in what will be committed (tracked files)
  $ git add <filename>

!) TAKING SNAPSHOT TO REPO:
> After the files have been staged, you can take snapshots of them using the git commit command.
  $ git commit

!) GIT COMMANDS YOU NEED TO KNOW:

  git config = Sets general Git parameters like username and email
  git init = Creates a Git repo within the current directory (also creates .git folder)
  git add <filenames> = Adds the specified filenames to the Git index (called staging)
    git add * = Adds all filenames to the Git index (called staging)
  git rm <filenames> = Removes the specified filenames from the Git index
  git commit -m <description> = Creates a snapshot/commit with a specified description
  git status = Views the status of a repo
  git log = Views the commit history of a repo
  git reset --hard <commit_ID> = Reverts files within a repo to a previous commit

  git clone /path = Clones a local Git repo to the current directory
  git clone username@hostname:/path = Clones a remote Git repo to the current directory
  git checkout -b <branchname> = Creates a new branch, and switches to it
  git checkout <branchname> = Switches to a different branch
  git branch = Views branches in the repo
  git branch -d <branchname> = Deletes a branch
  git push origin <branchname> = Pushes a branch to the original repo location
  git pull origin <branchname> = Pulls a branch from the original repo location

!) MY FIRST COMMIT:

  $ git init
  $ git add README.md
  $ git commit -m "first commit"
  $ git remote add origin https://github.com/PLeoK/Bash-My_Scripts.git
  $ git push -u origin master

=== Documentation / Articles ===
[1] https://tinyurl.com/yyhvdqan | Talk Tech to Me: Managing Linux Shell Scripts Using Git
