## Issue 431
<b>Ques - 3 Does the merge conflicts come when you applied your stashes? Why/Why not?</b><br>
No, the merge conflicts did not arise, because I added the 3rd question in the beginning of this file.<br>

<h3>Issue 409</h3>
<b>Ques - 1 How and why merge conflicts arise?</b><br>
When git is unable to resolve the difference between two commits while merging those commits, a merge conflict occurs. <br>
When all the changes in the two commits occur on different lines or in different files, Git will merge the changes without any conflicts. However, when there are changes in the same lines, git can't figure out which code to keep and which to discard and thus asks the user to resolve it.
Amerge conflict can arise in merging a branch, rebasing a branch or cherry picking a commit.

Hello! This is Aviral Gupta. I am a 3rd year student at IIITA.<br>
Repo URL: https://github.com/aviralgupta752/GoGit.git

<b>What do you really understand from SSH keys? What are the advantages of using it?</b>
SSH(Secure Shell) keys are an access credential that us used in the SSH protocol. While working with github, we need to verify ourselves using our username and password. SSH key is an alternative way to verify ourselves.<br>
SSH keys are more difficult to hack than passwords and thus are more secure.

To edit the last commit message one must use ```git commit --amend``` comand.

<h3>Issue 334</h3>
first commit

second commit:<br>
Steps:<br>
I have removed the first commit.<br>
Step 1: Finding the commit before the first commit using git log<br>
Step 2: Checkout that commit using git checkout<br>
Step 3: Make a new branch using the current checkout commit git checkout -b new_branch<br>
Step 4: Adding the commit after the removed commit git cherry-pick<br>
Step 5: Resolving merge conflicts and pushing our changes.<br>
Step 6: Double checking everything using git status.<br>
Step 7: Finally, switching to the original branch and performing a hard reset to the commit prior to first_commit using git reset --hard<br>
Step 8: Merging new_branch using git merge new_branch<br>
Step 9: Force pushed the changes in the repo using git push --force origin main<br>

<h3>Issue 397</h3>

<b> Ques - 1 Which kind of development(s) do you do? (web/app/cc/etc).</b><br>
Competitive Coding.<br>

<b>Ques - 2 Resources that you follow to learn the above tech-stacks (development)?</b><br>
Youtube, GFG for concepts and leetcode, codechef for practice.<br>


<h3>Issue 409</h3>
<b>Ques - 2 Is force push a good practice? Yes/No why? In most of the tasks on this repo, you used force push, so why this practice is Okay (neither good nor bad) in your case?</b><br>
No, force push isn't a good practice because after force pushing all the changes made by other members will be lost. <br>
Since, I have a local copy of the repo and I am the only one making changes to that repo, force pushing is okay.<br>

<b>Ques - 3 Name anyone Git or Github topic on which any issue is not made on this repo. (Your answer should be different from others.</b>
A task to modify the info.md to better looking and informative.(Will help in learning basics of HTML and also how to add tags and images in info.md)

```git tag``` command to give tags to specific commits.

<b>Ques - What changes to your procedure of doing this task will happen if I told you to write all first three answers (Ans - 1, 2, 3) at the end of the file.</b>
Since, there were only 3 answers, I made the changes manually by pasting each question again and making the commits.<br>
If ```git add -p``` were to be used:<br>
1. there would have been 2 hunks in this issue, and only the 2nd hunk would have to be manually edited.<br>
2. if all the answers were at the end of the file, there would have been only one hunk, therefore this hunk would have to manually edited 3 times.

## Issue 431
<b>Ques - 1 Why do we do fetch before the merge or pull?</b><br>
Before working on a new feature, we generally would want to work on top of the features already made by other contributors. To retrieve these changes from the remote repo, we do a fetch & merge or pull.


## Issue 443
<b>Ques 2 - What are Git Submodules? Why are they used?</b><br>
Git Submodules allows us to keep a git repo as a subdirectory of another git repo. They enable a Git repository to track version history of external code.<br>
Main use of it I found was to integrate the work of two different parties. One can also track changes in several repositories via a central one repo.

<b>Ques 1 - Why would one ever need to ever reorder his commits?</b><br>
Reordering of commits is done, if the commits makes more sense in reordered form or if the commits are to be squashed.
