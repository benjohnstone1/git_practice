Hello Git and Github

## Setting up new project ##
1) Create local directory and project
2) Create new repository in Github
3) Create remote and run terminal commands to push from local files to remote - using git push

## Backtracking in Git ##
Head commit (In Git, the commit you are currently on is known as the HEAD commit. In many cases, the most recently made commit is the HEAD commit.)

1) git show HEAD

Git Checkout (What if you decide to change the ghost’s line in the working directory, but then decide you wanted to discard that change?)

1) git checkout HEAD filename

Git reset - What if, before you commit, you accidentally delete an important line from scene-2.txt? Unthinkingly, you add scene-2.txt to the staging area. The file change is unrelated to the Larry/Laertes swap and you don’t want to include it in the commit.
We can unstage that file from the staging area using

1) git reset HEAD filename
2) git reset commit_SHA #(can reset the Head to a previous commit, supply first 7 digits of commit)

## Git Branching ##

1) git branch // tells you which branch you are on
2) git branch new_branch // create new branch called new_branch
3) git checkout branch_name // switch branch
3) git merge branch_name // merge giver branch into receiver branch

In our case if we had a separate branch we would first checkout the master branch then call git merge branch_name
This is "fast forward" because Git recognizes that branch_name contains the most recent commit (what if it didn't?)

Merge conflict (e.g. if had committed a change in master first)

Like this!


## Git Teamwork (Push, Pull) ##