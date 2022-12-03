# Инструкция по работе с git

Git - it's a program...

## Creating new repository

To create new repo(init)
need enter comand:
    
    git init

## Show the working tree status

Displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git

    git status

# Add file contents to the index

This command updates the index using the current content found in the working tree, to prepare the content staged for the next commit.

    git add<name>

## Record changes to the repository

Create a new commit containing the current contents of the index and the given log message describing the changes.

    git commit
$$OPTIONS$$

-m 

--message

    Use the given <msg> as the commit message. If multiple -m options are given, their values are concatenated as separate paragraphs.

-a

--all

    Tell the command to automatically stage files that have been modified and deleted, but new files you have not told Git about are not affected.

