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

## Git branches


### All branches viewing

To view all branches in repository you need to enter:

    git branch

### Branches adding

To add new branch use:

    git branch <branch_name>

\<branch_name\> - new branch name

### Branch merging

Incorporates changes from the named commits (since the time their histories diverged from the current branch) into the current branch. This command is used by git pull to incorporate changes from another repository and can be used by hand to merge changes from one branch into another.
Command to use: 

    git merge branch_name

### Merging conflict

During a merge, the working tree files are updated to reflect the result of the merge. Among the changes made to the common ancestor’s version, non-overlapping ones (that is, you changed an area of the file while the other side left that area intact, or vice versa) are incorporated in the final result verbatim. When both sides made changes to the same area, however, Git cannot randomly pick one side over the other, and asks you to resolve it by leaving what both sides did to that area.

### --graph flag info

<<<<<<< HEAD
Draw a text-based graphical representation of the commit history on the left hand side of the output.
=======
Draw a text-based graphical representation of the commit history on the left hand side of the output. This may cause extra lines to be printed in between commits, in order for the graph history to be drawn properly.

When --graph is not used, all history branches are flattened which can make it hard to see that the two consecutive commits do not belong to a linear branch. This option puts a barrier in between them in that case.
>>>>>>> graph_flag
