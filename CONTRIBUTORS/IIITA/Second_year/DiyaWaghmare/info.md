1. Merge conflicts arise when there are two different changes on the same line or same section of code so Git can't tell which chnages to include and which to remove.

Hey, my name is Diya Waghmare. 
I am a developer and student of IIIT Allahabad. 
My Github profile link is: https://github.com/diyawaghmare 
Online courses: https://sapient.udemy.com/course/the-complete-web-development-bootcamp/learn/
SSH keys are helpful so you don't have to write your username and password everytime you push to github and authenticate it. The randomly generated SSH key also makes it harder to hack and is safer to use. This is because there exists both a public and a private key, which should be stored safely by the user. It is a convenient and secure method.

Method to amend the last commit:
Type git commit --amend (If you want to open the editor and type new commit msg by entering insert mode)
or else Type git commit --amend -m "New commit msg" 
Web Development
Method to delete last commit:
git reset commitid^ --hard (Reset the branch to the particular commit)
git push origin -f (Force push it to remote repository)

2. Force pushing is not a good practice because it may cause conflicts for others working in that repository and it may overwrite someone else's commit. When we did it was fine because we were the only ones working on our repositories.

3. git bisect, git hooks, git submodules

If we had added all 3 answers at the end we would have only one hunk to edit while adding commits intsead of two hunks.

1. Create a merge commit: In this method, an extra merge commit will show along with all the other commits in that PR in our commit history. This extra merge commit gives details about which branch is being merged.
2. Squash and merge: There is no extra merge commit in this method as all the commits in that PR gets squashed along with it. There is an option to change the commit message so that we will see only one commit in our commit history.
3. Rebase and merge: This method rewrites git history to append changes from the branch individually, without creating a merge commit. This method should be used carefully.
4. Merge locally: In this method you can use your command line to merge commit. After fetching remote, we use git merge --no-ff to prevent fast-forwarding a commit. This works like the 1st method and adds an extra merge commit.

The first method in which we create a merge commit is the best way to do it because you can clearly see all the commits (helpful in instances where you need to find a bug) and the commit history isn't altered either.
We would have to reorder our commits so that it could be interpreted better in the Github commit history (it might make more sense in a different order).
Ques 3. Yes I will get merge conflicts because I've written the answer for ques 1 and ques 3 in the same section of my markdown file.
We use git Submodules when we might need to use the contents of one repository in another so we make that repository a sub directory(submodule) in the main repo.
Ques 1. Git pull doesn't let you review the changes that you are pulling from the remote repo to your local copy. Fetching changes allows us to review those changes before merging or pulling them (otherwise we may lose the changes in our local copy and they may be overwritten).

Forking is always recommended as it allows you to make changes without affecting the remote repository and can be reviewed before merging it. We can't directly clone and then merge if we are not a contributor in that particular repo with commit access and permission to create branches.

Yes, we can undo a hard reset of a commit using reflog (to see a list of all the changes made in your branch recently). GitHub has the history of all the commits and we can find the commit that we had reset and undo it.

Second half
Ques - 2 Explain in detail the difference between HEAD, working tree and index, in Git.
Ans. Working tree is nothing but the files you are currently working on where we can try out any chnages we want. After we are done working on our files we move it to our staging area to be committed (index).

HEAD is a pointer to the branch or commit that you last checked out, and which will be the parent of a new commit if you make it.  For example, if we are on the main branch then our HEAD will point to to the last commit made in the main branch. Once we commit, main will be updated to point to the new commit. So it is the current commit you are working with and is usually a "branch head". If you checkout (and work on) any commit which isn't one of the (branch) heads, you are in a "detached HEAD" mode.

The index is an alternate name for staging area where the new commit is prepared. Once our filed are staged from the working tree into our index, their contents can be committed. If we do git commit -a, this will automatically add all changes to files that Git knows about to the index before committing, so it will commit the current contents of your working tree as well.

For more information, you can read from https://www.py4u.net/discuss/1720480