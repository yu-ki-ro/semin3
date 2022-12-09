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

## Show commit logs
Shows the commit logs.
    
    git log

$$OPTIONS$$

--oneline

    This is a shorthand for "--pretty=oneline --abbrev-commit" used together.
-add

    It shows all commits in the history of branches, tags and other refs, but it does not show commits that are not reachable from any ref. A typical example of a commit that is not reachable from any ref is when you've just run git commit --amend: the previous commit still exists locally, but it's no longer reachable and won't be shown in git log --all. But git reflog will confirm that it does indeed still exist.

![Git image](fengmian.jpg)

## Ветвления

Ветвления в гит нужны для ...

## Отображение всех имеющихся веток
 Для показа всех веток используеться команда:
    
    git branch

### Создание новой ветки

чтобы создать ноаую ветку

### Переключение между ветками

 чтобы переключиться на новую ветку

## Description of commands

### git branch  daw

    The git branch command is the main tool for working with branching. You can use it to add new branches, list and rename existing ones, and delete them.

### git branch -d <name> dwad

    remove branch with a <name>

### git checkout <branch_name> 1w2

    To prepare for working on <branch>, switch to it by updating the index and the files in the working tree, and by pointing HEAD at the branch. Local modifications to the files in the working tree are kept, so that they can be committed to the <branch>.

### git log --graph
    
    The --graph flag enables you to view your git log as a graph. To make things things interesting, you can combine this command with --oneline option you learned from above.

### git log --all --oneline --graph

    The ---all --oneline --graph flag causes git log to display
    
    all commits
    one commit per line
    the first seven characters of the SHA
    the commit message
    view graphs

### git merge

    The git merge command merges the individual development directions created with the git branch command into a single branch.
    