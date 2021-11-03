Hello,
My name is sai sumanth kumar
My repo link is <a href="https://github.com/saisumanthkumar/GoGitTestFile">Here</a>

### Ques - 1 What if you clone without fork? What problems will you face when you try to contribute in this condition?

**Ans-1** When we clone the repository without fork,the changes will be pushed to main repository but this is not possible if we dont have the access to the repo so we make a copy of the repo and push changes into it so that the owner of the repo can verify our contribution and merge it.
The main point to note here is that any changes made to the original repository will be reflected back to the forked repository. However, if you make any changes to the forked repository we will have to explicitly create a pull request to the original repository.

### Ques - 2  Can we undo a hard reset of a commit? If No/Yes why? (Undo means can we get back the changes that we did in that commit?)

**Ans-2** yes we can do a hard reset and get the commits back. As Git stores all the history of every event permanently. The event related to the HEAD are stored as references in `.git/refs folder`. We can view the reference logs using : `git reflog`
This will show all the changes that occured. Now we can copy the commit hash of the commits we want and the can use cherry-pick to get the changes back.

### Ques - 3 Explain in detail the three-stage architecture of Git.

**Ans-3** Git is three-stage architecture those are 
- Working directory
- staging area and 
- Git Repository
Working directory is the file explorer’s folder where the files are stored, Staging area is a area where those files are present which we want to send to commit, After commit is fired, files which are in staging area will move to Git Repository.