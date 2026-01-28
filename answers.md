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

