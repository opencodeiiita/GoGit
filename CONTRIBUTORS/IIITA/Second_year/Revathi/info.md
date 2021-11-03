SSH keys:
SSH is a secure shell network protocol that is used for network management, remote file transfer, and remote system access.
When SSH is created a public and a private key is generated. public key(lock) is shared with a platform and private key(key) is kept to oneself in a secure place.
SSH is a total solution to allow trusted, encrypted connections to other platforms.

How to edit the last commit message in git?
Ans:The most recent commit message can be edited using the git commit --amend command 
git commit --amend -m "title" -m "description"
use force push to change a commit which has been pushed.

Ques - 1 What if you clone without fork? What problems will you face when you try to contribute in this condition?
Ans: When we clone without fork the changes we make will be pushed to main repository but this is not possible if we dont have the access to the repo 
so we make a copy of the repo and push changes into it so that the owner of the repo can verify our contribution and merge it.
Ques - 2
In most of the cases we can change it depends on the state your repository. 
the effects of git reset --hard can range from trivial to undo. 
you can recover commits using git reflog it shows the list of times when head is changed. 
We can use git reset --hard commit-id to undo the changes. 

three-stage architecture of Git.
The three stages of git architecture are working directory, staging area, git repository.
Working directory is the directory which contains our local file
Staging area has only those files which we have staged and  are needed to be commited, once we are sure we can commit 
and push our changes to the remote repository.
Git repository is where all the collaborators push their works and we can get their working by pulling to our local directory

