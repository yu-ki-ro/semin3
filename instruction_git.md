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

## Show changes between commits, commit and working tree, etc

Show changes between the working tree and the index or a tree, changes between the index and a tree, changes between two trees, changes resulting from a merge, changes between two blob objects, or changes between two files on disk.
    
    git diff

This form is to compare the given two paths on the filesystem.

    git diff <hash1> <hash2>

## Switch branches or restore working tree files

Updates files in the working tree to match the version in the index or the specified tree. If no pathspec was given, git checkout will also update HEAD to set the specified branch as the current branch.
    
    git checkout <hash>

