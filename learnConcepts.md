'Crucial consepts of Git'
## OFTEN FOR A SIMPLE WORK IS ENOUGH TO DO:

```git add .
git commit -m 'describe shortly'    
git push origin master``` 


# some basic terms:
0. gitignore - a way to avoid pushing some credentials or secret stuff when pushing chnages to remote. 
1. repository
2. clone
3.push or pull
4. pull request. Merge. Open a pull request. 
# Saying will you please take those changes from created branch and merge them into master.
# comments 
5. master, branches, ...
# the moments of each commit has uuid. If I'm not sure that I want to edit my master branch.
6. commit (like save but having his own unique identifier - hash)
7. the line for some concept I don't remember.
8. another line for a consept I can't remember. 
These are the concepts that is good to know. 
9. MASTER IS ALSO GETTING SOME CHANGES.
10. update git clone
if fetch + merge : 
`git pull`
else 
`git fetch`

git commit is explained if you execute the following command on git bash:
`git`

# get changes from remote into your local catalog:
`git fetch repourl`
`git merge origin/master`
    
if you cloned and changed cloned repo locally the you neeed changes be reflected 
in git it means you need to push to remote 
remote is github repo
`git remote -v`


## How to create a pull request of the edited master branch in order to reflect changes in forked branch.

I used create pull request and switched branched I wanted to get changes in On b.anch alex_k_work.

## how to push changes made locally when some files in you remote are also edited

    Create a new branch:
    git checkout -b feature_branch_name
    Edit, add and commit your files.
    Push your branch to the remote repository:
    git push -u origin feature_branch_name
## why not to checkout a new branch?

`git checkout -b content`


## turn subfolder into a new repo

https://help.github.com/en/github/using-git/splitting-a-subfolder-out-into-a-new-repository


<https://github.com/mattharrison/Git-Supervisual-Cheatsheet>

## Git tips

    1. When working with multiple branches you can stash changes away that you are not yet ready to commit:

    git stash save "save message"

    You can then retrieve them later with:

    git stash list
    git stash pop <stash_item_hash>

    2. When you want to add more changes to the last (local) commit, use:

    git add file(s)
    git commit --amend

    This opens your editor and lets you modify the last commit.

    3. On the other hand, if you want to spread out your changes over multiple commits (granular commits are good!), use:

    git add -p

    Here you can commit only parts ("hunks") of your changes in interactive mode.

    4. Imagine you get excited coding, and accidentally commit your changes to the main branch. No worries: if you forget to branch off earlier, you can still do so at this point:

    git branch new_branch

    Now you have your changes on both the original and new branch so you can wipe them out on the former:

    git checkout original_branch
    git reset HEAD~<number-of-commits-to-go-back>

    (Make sure this is all local though, don't go modifying changes you already pushed!)

    5. If you want to use a commit from one branch on another, you can cherry pick it:

    git cherry-pick <commit_from_anywhere_in_your_repo>
