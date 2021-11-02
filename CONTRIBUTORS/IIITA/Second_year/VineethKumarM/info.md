q1: when there are different changes in the same part of the file, git doesn't no which change should be merged 
so it presents us the merge conflicts.

Hi there!<br>
It's Vineeth Kumar Munigyala this side<br>
My Github Handle [VineethKumarM](https://github.com/VineethKumarM)<br>
The Repo I created for this task is [here](https://github.com/VineethKumarM/Sample-Repo-for-GoGit)

Ques - What do you really understand from SSH keys? What are the advantages of using it?
ANSWER: ssh keys are used for authentication, these help us to connect to github without using our credentials everytime. It has a pair of values of which only one, the public key will be stored in our local system and used for encryption.
Ques - How to edit the last commit message in git?
ANSWER: A simple way is to use the following command: 
		git --amend -m "title" : to only edit the title
		git --amend -m "title" -m "description" : to add description also
		to edit a commit after pushing to github repo we shoulg use push --force--with--lease which will help us not to lose others commits if pushed in the mean time.
		*amend can only be used to edit the most recent commit messags*
Ques - Which kind of development(s) do you do?  =>  ANSWER: WEbD
Ques - Different delete task
ANSWER: as per the instructions i will be making 2 commits and i will remove/delete the second commit 
	I wiil be using a different method here 
	1. make two commits
	2. i will discard the second commit using te "git revert <commit hash>"coomand
	3.but revert will itself make an extra commit so i will squash all this into first commit using git rebase and by replacing pick with squah keyword and then push again




Ques - Resources that you follow to learn the above tech-stacks?
ANSWER: Youtube, Udemy and sometimes articles/blogs on the Internet.


q2: force push is not recommended. when we force push git overwrites the recent commits,
it may result in loss of others work.we have used force push in the gogit tasks as only I am working in my repository.


q3: git submodules.




q4: there wont be much change in the procedure, if we added all answers at end then we are presented a 
single hunk to edit. then we would have separated that hunk into three and make the respective commits
one by one.



Different types of merging pull requests
pr made to master branch
Create a merge commit:
this will add all the commits from the pr, and makes an additional merge commit with the details of the merge in our master branch. This is very simple and the default option on github. 

Squash and Merge:
It squashes all the commits into one and merge's it without any merge commit.
before squashing we can provide a squash description also.For example smaller commits that are added to keep track of work being done that don’t necessarily need to have their own commit, we can instead squash them into one commit. 
> But when mentors can use this to merge prs why did they ask us to squash🤔🤔.

Rebase and Merge:
It adds all the commits from the pr to our repos history. There is no extra Merge commit. The most recent commit of the pr 
will now be the HEAD of our master branch. Rebases set the committer of the rebased commits to the current user. But this can be done only when there isn't any merge conflict.

only the ones with write access to the repo can perform the above tasks. And if only that specific type is enabled for that repository.

Merge locally through command line:
I hope this is the best method for repo's that maintain any development project.
In this method for a specific pr we use the pr ID and fetch it into a new branch. using the command :
*git fetch origin pull/ID/head:new-branch-name* then checkout to that branch . Now we can test the changes and we can edit the changes too. after reviewing we can checkout to the master branch and merge this new branch: *git merge --no-ff new-branch-name*
the flag is added so git dont make a fast forward merge. then we can push our changes to the remote. The pr will automatically be closed. 








Ques - 1 : When you clone someones repo without forking it, the original repo will be set as the remote to your local repository.
We know that to share our work with colleagues who are working within the same repo, we add a remote and push our changes, and we fetch 
others changes. Now while contributing when you neeed to push the commits we get a permision error unlesss you have the write access to the original 
repository. So if are not one of the collaborator you cant contribute. If we had forked the repo initially we wont face this issue as we can push commits to our fork and make a pr.


ques2 : Yes, depending on the changees of the repo we can undo a hard reset of commit. We can find the details of the commit in git reflog. Using the commit id of the commit which is before our hard reeset we can undo the changes.
use git reset --hard commit-id.
we cannot undo a  reset which erased unstaged changes but we can undo one that has erased commits and staged changes.





