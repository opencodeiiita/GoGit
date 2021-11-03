
Ques - How and why merge conflicts arise? 
Ans - A merge conflict arises when two branches both modify the same line(s) of a file and are subsequently merged. Git can't know which of the changes to keep, and merge conflict arises.

Ques - Above, I told you to merge branch-1 into main, tell me which type of merge is this and why? Also, explain it too.
cc
Ans - This above type of merge is fast forward merge because there are no commits made on main branch after commiting in branch-1 when there are commits made on master branch after commiting on branch-1 then recursive merge occurs and there might be some merge conflicts.

Ques - What do you really understand from SSH keys? What are the advantages of using it?
seniors
Ans - A SSH key is a substitute way of distinguishing ourself.It converts out password into 256 byte token which makes it impossibe to find by recurssion hence impossible to hack. SSH keys come two by two, a public key that is accessible to everyone and a private key that is put away just on your PC.It is used to encrypt it(by using public key) and decrypt(only by the private key) so that the info. between them gets secured, and pass through secured channel
 
Ques - How to edit last commit message in git?

Ans -  To edit our last commit message in git we have to use a command "git commit --amend", this will show us the last commit message int vim we can use insert and edit our commit message hit :wq exit the vim and hence last message is commited

Ques - How to delete a commit in git?

Ans -  To delete a commit in git we have to use a command "git rebase -p --onto SHA^ SHA",ShA can be found out by git log 

Ques - Is force push a good practice? Yes/No why? In most of the tasks on
this repo, you used force push, so why this practice is Okay (neither good
nor bad) in your case?
Ans - Force push may be good or bad. We should never ever force push on a
public repository because this can break someone's pull.
Because this is a forked repositry of the main repositry force pusing it 
doesnt break any pull hence no problem occures.


Ques - Name anyone Git or Github topic on which any issue is not made on this repo. 
Ans - Working on remotes.


Ques - What changes to your procedure of doing this task will happen if I told you to write all first three answers (Ans - 1, 2, 3) at the end of the file.

Ans - If we write at the end then we have to edit 1 hunk but by this method we have to edit 2 hunks





Ques - Explain all these 4 different kinds of merge that you performed above and how a particular method is different from the others. What are the pros and cons of a particular method and some other similar things? In short, you have to differentiate all these 4 different kinds of methods. Also, tell that in general out of these 4 methods, which one is best and why?

Ans - 
1) merge commit: 
Using this merge method all the commits made in the branch are merged onto the base branch with a merge commit .

2) squash and merge: 
Using this merge method, all the commits of the branch are squashed into one commit and then we need to choose the commit name and then these all commits are merged into the branch which we are creating pr without a merge commit.This requires the squash commit access to merge the pr.

3) rebase and merge:
Using this merge method all the commits of the branch are added to the base branch individually without a merge commit. The rebase and merge method modifies git commit history, therefore should be only used for small changes. 

4) Terminal merge: 
Using this method helps in merging commits using our terminal first we have to make sure the head of the branch which is getting meged is updated to avoid any conflicts then we can use have to go to that branc and use git merge --no--ff <branch name> to add a merge commit or git merge <branch name> to merge without a conflict
