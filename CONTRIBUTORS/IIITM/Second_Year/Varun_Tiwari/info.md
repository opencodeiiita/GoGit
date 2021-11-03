ans-1 : it arises when git cannot merge changes automatically. like while doing the cherry-pick task, we faced merge conflicts because while cherry-picking we changes the text in the same lines and git cannot understand which change to  preserve while merging. 

### Hey, I'm Varun Tiwari
I am a student of ABV-IIITM, Gwalior.
To know more about me [visit here](https://github.com/varunKT001)
This is the link of the repo [GoGit_repo](https://github.com/varunKT001/GoGit)

## Issue : 223 
#### Ques - What do you really understand from SSH keys? What are the advantages of using it?
SSH keys are just pairs of a public and private key. The Private keys are used to encrypt/decrypt the user identity. SSH keys provide more security as well as convinience to the user.  

## Issue : 332 
#### Ques - How to edit the last commit message in git?
There are two cases : 
1. Changes not pushed : If changes are not pushed we can simply add --amend flag and it will amend last commit. 
2. Changes are pushed : If Changes are pushed we need to --amend the and also force push the changes using the -f flag

## Issue : 366
First commit. We will go to the file state in first commit and checkout to new branch. then we will come to master and hard reset to the previous branch head.

ans-2 : yes. force pushing is bad practice because it modifies git history and lead other users become out of sync. We may overwrite someone else's commits and cause merge conflicts for others. It did'nt cause any problem in our case because we were the one working on our repositories.  
ans-3 : I think the git bisect isn't used in any task. 
top commit : If we had all the three ans at the end of the file, we would need to manually edit the hunks to only contain one answer and then commit the changes.




web developement









youtube: freecodecamp


so first I used git log to see the last commit on 14 october because we know that no bug was there at that time
Then I copied the commit hash of the last commit of 14 october and used: 
git bisect start HEAD <commit hash>
This starts git bisect and test each commit for a bug. we will use
git grep 'bug'
this will find all files by matching if file contains 'bug'.
If we do not find a file we will tell bisect to mark the commit as good: 
git bisect good
But if we find the file with bug, we will use
git bisect bad
Upon finding a bad commit, git puts us on the same commit we marked bad
then we can copy the commit hash and use
git bisect reset
This will put us on the head from where we started
Now we can revert the changes of the bad commit using 
git revert <bad commit hash>
This is the best method to find bug because we can move to individual commits and test the code for bugs and can revert the changes if bug is found. 


1. create a merge commit: 
In this merge method, all the commits of the branch, lets say test, are merged onto the base branch along with a merge commit which tells details about the merge like which users repo commits are merged. 
To use this method, we must have write permissions in the repo

2. squash and merge: 
In this merge method, all the commits of the branch, lets say test, are first squashed into one commit and then are merged onto the base branch (without a merge commit). 
To use this method, we must have write permissions in the repo and the repo must allow squash merging. 

3. rebase and merge:
In this merge method, all the commits of the branch, lets say test, are added to the base branch individually (without a merge commit). The rebase and merge method modifies git commit history, therefore should be only used for small changes. 
To use this method, we must have write permissions in the repo and the repo must allow rebase merging. 

4. manually merging using terminal: 
In this method, we use our terminal to merge a pull request.
Firstly we will fetch the remote data onto our local system using: 
git fetch origin
Now we will checkout to a new branch with the head pointing to origin/test, say test, using:
git checkout -b test origin/test
Now we will merge the base branch to test using:
git merge main
Now checkout to main branch: 
git checkout main
Now we can merge the branch test to base branch main using: 
git merge test
OR
git merge --no-ff test
If we use the first command, there will be no merge commit, but if we use the second command, there will be a merge commit. 
Now we can push the changes to the remote: 
git push origin main

Commands used by me for the 4th method (branch b4 already exist on my local system):
(already merged previous 3 branches to main-copy) 
git checkout main-copy
git pull origin main-copy
git fetch origin
git checkout b4
git merge main-copy
git checkout main-copy
git merge --no-ff b4
git push origin main-copy

Ques - 3 Does the merge conflicts come when you applied your stashes? Why/Why not?
Yes, they came. Because I answered the question 1 and added question 3 at the same line. So when I tried to apply the stash second time, there was a merge conflict. I resolved the merge conflict and the committed the changes. 
Ques - 1 Why do we do fetch before the merge or pull?
while using git pull, git takes the changes on the remote repo and tries to automatically merge them to our local copy. But if we want to review the changes first, we cannot do that with git pull. That's where we use git fetch. git fetch command searches for changes and commits on the remote (which are not on our local copy) and saves them without automatically merging. We can review the changes before we merge them. 

Ques 1 - Why would one ever need to ever reorder his commits?
ans : sometimes a particular order of commits make more sense. It may used when we need to push only one commit to the remote.

Ques 2 - What are Git Submodules? Why are they used?
ans : git submodules is a record in our repository which is pointing to a specific commit in some other repository. In some cases, where the external repository changes very frequently, incorporating changes may become difficult and could also break our application or api. Thats why we use git submodules to point to a specific commit and lock its code at a particular commit. 

Ques - What is a GitHub gpg key? Why it is used? Also, tell that why we need to sign the commits?
ans : github gpg key is a public key used by github to verify the signature of the commits. When we sign a commit using our private gpg key and push the changes to github, github first checks the signature using the public gpg key, and if the signature is verified, we get a verified commit. Signing commits is important so as to verify the identity of the commiter. 

Q1 - Explain objects and refs folder inside ./git. Where git commits are stored in ./git folder?
ans : every event in git is saved as a hash value in object folder. It stores the data about what are the files, where are the located, etc. In git, we deal with commits, be it in main branch or some other branch. Inspite of using commit hashes, we can specify a commit reference. For example : 
To go back to a commit we can use => git checkout <COMMIT_HASH>
Or we can use the same checkout command by specifying a branch name => git checkout <BRANCH_NAME>
So the branch name is just a reference to a commit on top of that branch. The ref folder inside .git folder is used to store these references. 
As said earlier every event is stored as a hash in object folder, so all the commits also reside here. 

Q2 - Differentiate between tree and blob in git? What they represent?
ans : the working tree in git is the directry in which all our files are placed. whenever, there is any change in the tree, git index the changes and we can then stage and commit them. 
A blob is a type of object used to store the contents of each file in a repository. the blog contains the hash of the files. these blobs are used by git to track and store changes in the working tree.

Ques - 1 What if you clone without fork? What problems will you face when you try to contribute in this condition?
ans : cloning is simply get a copy of the remote repository to the local system, while forking creates a copy as well as maintains sync with the original repository. If we clone without fork, I become dificult to sync the changes between local and remote. Also If we want to contribute to a project, just cloning is a bad choice. We won't be able to create any pull to the remote repository because we would not have any collaborators access. The owner of the repository needs to add us as a collaborator for us to make  changes. While in forking we can make our changes and create a pull request easily without and hassle. Also forking helps us maintain sync with the two repositories.  

Ques - 2 Can we undo a hard reset of a commit? If No/Yes why?
ans : yes we can do a hard reset and get the commits back. Git stores all the history of every event permanently. The event related to the HEAD are stored as references in .git/refs folder. We can view the reference logs using : 
git reflog
This will show all the changes that occured. Now we can copy the commit hash of the commits we want and the can use cherry-pick to get the changes back. 

SECOND PART: 
Ques - 2 Explain in detail the difference between HEAD, working tree and index, in Git.
Ans - The hierarchy followed in the three stage architechture of git is : 

WORKING TREE    INDEX      HEAD
    | --------->  |          |
    |(index file) | -------> |
    |             | (commit) |

Working tree : Working tree contains the file structure of our repository, i.e this is where all our files resides. It is the place where we make changes to our files (like coding a new feature, removing bugs etc.). After making changes we can move the desired files to the index (staging area). 

Index : Index is the list all the files whos changes are to be committed. All the files in the index will be used when you commit your changes, and are replaced by the original files before commiting. We can also remove some files from the index, make some more neccessary changes and add them to the index again. To add a file to the git index we use the following command :
git add <FILE_NAME> => this will add the specific file to the index
git add . => add all the files in the working tree to the index
To remove files from the index use the following commands : 
git restore --staged <FILE_NAME> => remove particular file from index
git restore --staged . => remove all the files from the index

HEAD : HEAD is a reference to the last commit made in the current branch. For ex : 
If we are on main branch then head will point to the last commit made in the main branch (here, 3)

(main branch)
1 --> 2 --> 3 (HEAD)
      |
      4 --> 5 --> 6 
      (dev) 

If we are on dev branch then head will point to the last commit made in the dev branch (here, 6)

(main branch)
1 --> 2 --> 3 
      |
      4 --> 5 --> 6 (HEAD)
      (dev)  

Also, head will be the parent of the next commit going to be made in the branch when a new commit is made the head will be updated that commit in the branch. 