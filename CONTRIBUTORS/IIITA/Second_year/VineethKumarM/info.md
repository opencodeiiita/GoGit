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