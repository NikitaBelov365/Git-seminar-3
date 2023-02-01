# Git instruction

![image](image.jpg)

## New repository created

To initialize new repository use:

    git init

## Repository status

To check current repository status use:

    git status

## Adding file contents to the index

To add/delete/change file content before commiting use:

    git add 'file_name'

## Recording changes to repository

To record changes to repository and to assign unique number to index use:

    git commit

## Adding commit message

To bind some message as a commit message use:

    git commit -m 'message'

## Merging add + commit in one command

If you need to instantly commit added changes use:

    git commit -a

## Merging add + commit + message in one command

Best way to instantly commit changes that you added and to apply some description is using next command:

    git commit -am 'message'

## Listing commits

To list commits that are reachable by following the **parent** links from the given commit(s) use:

    git log

## Log flags

### Displaying logs in compact format

To view commit log in compact format use next flag:

    git log --oneline

### Listing all commits

To list all commits including those that were made after HEAD use:

    git log --all

### Listing all commits in compact format

If you want to see all commits that made before and after HEAD in compact format use:

    git log --all --oneline
    
## Displaying difference between actual index and last commit

To show changes between actual index and last commit use next command:

    git diff

## Switching branches

To switch branch by the commit number use:

    git checkout commit_number