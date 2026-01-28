# Git exo — Answers

## Part 1: Setup & config
- Git version: `2.52.0'
- Config commands used:
  - git config --global user.name "Ditri Collaku"
  - git config --global user.email "ditri.collaku@student-cs.fr"

## Part 2: Create Your First Repository
Commands used:
- mkdir my-first-repo
- cd my-first-repo
- git init
- touch README.txt

## Part 3: Your First Commit

- Command that shows the current state of the repository:
  - git status
- Command that stages readme.txt for commit:
  - git add readme.txt
- Command that commits with the message "Add readme file":
  - git commit -m "Add readme file"
- Command that shows the commit history:
  - git log

## Part 4: Make Changes

After editing README.txt, git status shows that the file has been modified
but the changes are not staged yet. This means Git sees the change, but it
will not be included in a commit until it is added to the staging area.

Number of commits so far: (5)

## Part 5: Exploration

- git diff:
  Shows the differences between the working directory and the last commit.
  It helps see what has changed before committing.
- git log --oneline:
  Shows a simplified view of the commit history with one commit per line,
  including a short commit hash and the commit message.

## Part 6: Working with Branches

- Command to list all branches:
  - git branch
- Command to create a new branch called feature-script:
  - git branch feature-script
- Command to switch to feature-script:
  - git switch feature-script
- Command to create and switch to a new branch called dev:
  - git switch -c dev
- Command to switch back to feature-script:
  - git switch feature-script
- To verify the current branch:
  - git status or git branch

## Part 7: Bash Script on a Branch

- Created install.sh on the feature-script branch
- Added a shebang line
- Printed start and end messages
- Updated package list and installed a package
- Made the script executable
- Committed the script to the feature branch

## Part 8: Merge Branches

Before merging, install.sh was not present on main because it was created on the feature-script branch.
After merging feature-script into main, install.sh appears in the directory.
The commit history now includes commits from both branches.
The feature-script branch was deleted after merging.

## Part 9: Push to GitHub

- Command that links local repo to GitHub:
  - git remote add origin https://github.com/ditricollaku/my-first-repo.git
- Command that pushes commits to GitHub:
  - git push -u origin master
After refreshing GitHub, I can see my files and commits on the repository page.

## Part 10: Delete and Clone

- Command to delete the local repository folder:
  - rm -rf my-first-repo
- Command to clone the repository from GitHub:
  - git clone https://github.com/ditricollaku/my-first-repo.git
After cloning, I navigated into the folder and verified the files were present using ls.

