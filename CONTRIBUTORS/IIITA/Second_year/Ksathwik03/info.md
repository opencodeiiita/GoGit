
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

