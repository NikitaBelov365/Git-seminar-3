# Git instruction

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

    commit

## Adding commit message

To bind some message as a commit message use:

    commit -m 'message'

## Merging add + commit in one command

If you need to instantly commit added changes use:

    commit -a

## Merging add + commit + message in one command

Best way to instantly commit changes that you added and to apply some description is using next command:

    commit -am 'message'

## Listing commits

To list commits that are reachable by following the **parent** links from the given commit(s) use:

    git log