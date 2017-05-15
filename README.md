# Git-Exercises
A repository for teaching some of the basics of Git workflow.

## Exercise 2 - Merging, Rebasing and Solving Conflicts
### Setup
1. Create branches "Exercise2a", "Exercise2b", "Exercise2c", "Exercise2d" based off of the master branch
2. Pull each branch from this repository into each of your respective local branches
3. Take a mental note that you won't change anything on the a or b branches
4. Switch to branch C

### To Do
**Part A**
1. Using the merge command, merge the changes from branch A into branch C
2. Using the merge command, merge the changes from branch B into branch C
3. You will see a message about **merge conflicts** which means the same line in both files has been modified. To fix the conflicts, open up the files git complained about, search for the `<<<<<< [changes from one branch] ====== [changes from other] >>>>>>` lines. Figure out which changes are from branch A and delete the other lines between the `<<<<<<` and `>>>>>>` lines as well as those lines themselves.
4. Finish the merge.
5. Commit and push to a new branch here.

**Part B**
1. Using the rebase command, perform an **interactive** rebase of branch B onto branch D, and ensure to not include the "unwanted commit#" commits.
2. Rebase branch A onto branch B, again ensuring to not include the "unwanted commit#" commits.
3. Fix the conflicts, but this time preserve the changes from branch B instead.
4. Finish the rebase.
5. Commit and push to a new branch here.
6. Done!

## Exercise 2a,b,c,d - Merging, Rebasing and Solving Conflicts

### Git Command Reference
- change branches `git checkout [branch name]`
- create a branch based on current branch `git checkout -b [branch name]`
- check what files have been changed since last commit `git status`
- prepare file to be commited `git add [file path]`
- commit changes with message `git commit -m "[message]"`
- push changes of your current branch `git push origin [branch name]`
- merge a branch onto your current branch `git merge [branch name]`
- rebase your current branch onto another branch (your changes will start after the most recent changes on that branch) `git rebase [branch name]`
- rebase with interactive options to edit commits `git rebase -i [branch name]`
