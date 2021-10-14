Hello! This is Aviral Gupta. I am a 3rd year student at IIITA.<br>
Repo URL: https://github.com/aviralgupta752/GoGit.git

<b>What do you really understand from SSH keys? What are the advantages of using it?</b>
SSH(Secure Shell) keys are an access credential that us used in the SSH protocol. While working with github, we need to verify ourselves using our username and password. SSH key is an alternative way to verify ourselves.
SSH keys are more difficult to hack than passwords and thus are more secure.

To edit the last commit message one must use ```git commit --amend``` comand.

# Issue 336
first commit

second commit:
<b>Explain the whole process that you will be using to delete that commit.</b>
Using cherrypick to remove the commit.
Steps:
1. Finding the commit before the commit I wanna remove using ```git log```.
2. Checking out that commit.
3. Make a new branch
4. Add all the commits after the removed commit using cherrypick.
5. switch to original branch and performing hard reset to the commit prior to the commit I am gonna remove.
6. Merge the new_branch with this branch.
7. Force push the changes.
