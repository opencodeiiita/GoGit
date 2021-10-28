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


for copy4











