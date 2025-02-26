# Git Helper

## Getting Started
```bash
git clone https://github.com/CSUEB-Black-Jack-Group-5/CS401-BlackJack.git
```
- This will retreive the contents of the repository and make a new folder on your computer

## Basics of Git
```bash
git status                  # lists out the currently modified files
git add <file>              # adds a currently modified file to the "staging area"
                            # the file is not yet on the internet yet when doing this, you're simply staging
git commit -m "<message>"   # creates a commit of all the staged files on your local git repo
git push                    # finally, this pushes the commits onto github for all to see
```

## Things to remember
1. Before making changes to your local copy, make sure you `git pull` in case someone else has pushed since the last time you worked on the project

## Common situations
1. Lets say you're in a position where you've forgot to pull before editing, and when you try pushing your running into problems
```bash
git stash <changed_file>    # save your local changes on a stack
git pull                    # pull the changes from github
git pop                     # restore the saved changes (may run into merge conflicts)
```
   - Now you can continue as normal editing the SRS
