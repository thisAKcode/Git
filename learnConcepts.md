'Crucial consepts of Git'

ADD SOMETHING TO REMOVE LATER.
some basic terms:
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



10 update git clone
if fetch + merge : git pull
else git fetch

git commit is explained if you execute the following command on git bash:
    $ git

# get changes from remote into your local catalog:
git fetch repourl
git merge origin/master
    
if you cloned and changed cloned repo locally the you neeed changes be reflected 
in git it means you need to push to remote 
remote is github repo
git remote -v   

often for my simple beginner programs it is enough to do 

git add .
git commit -m 'describe shortly'    
git push origin master



# How to create a pull request of the edited master branch in order to reflect changes in forked branch.

I used create pull request and switched branched I wanted to get changes in On b.anch alex_k_work.

# how to push changes made locally when some files in you remote are also edited

    Create a new branch:
    git checkout -b feature_branch_name
    Edit, add and commit your files.
    Push your branch to the remote repository:
    git push -u origin feature_branch_name
## why not to checkout a new branch?

`git checkout -b content`


## subfolder into a new repo

https://help.github.com/en/github/using-git/splitting-a-subfolder-out-into-a-new-repository