Merge Conflicts arise when commits are added to the same place in a file, when they coincide.Suppose both the commits want to add changes to the same line, they are not overwritten by each other, and hence merge conflicts arise.
Hey!<br>
This is Raghav Goel.<br>
My  <a href = ""https://github.com/raghavgoel25"">Github Profile</a>

What do you really understand from SSH keys? What are the advantages of using it?

SSH key is a method that can be used for authentication different from normal passwords mainly in the way it operates. 
SSH keys are more long than typically used passwords and are computer generated, making them less prone to hacking. 
 They are not stored on servers, but only the device which is being used for login, hence again
making it less vulnerable to hacking.
 Github GPG keys are a way of verifying and signing your work. They can be used to encrypt and sign commits or tags to verify your respective contributions. It helps in verifying the identity of the person who made the commit.
 How to edit the last commit message in git?
 The following commands should be executed:-
 1.git commit --amend -m "New message" 
 2.git push --force repository-name branch-name
 If you are not sure whether someone has cloned your repository after your latest commit, instead of the second command, use.
 git push --force-with-lease repository-name branch-name
 This command will abort the push if there are any upstream changes to the repository, whereas the --force command will destroy any changes.
The main reason to reorder a commit is to improve your git history, so that when the commits are in 
a particular order, they make more sense to the user and to a person viewing it.
 How to delete a commit?
 I will use git reset --hard HEAD^ to delete the latest commit i will have made.
 Dependabot is a github feature that helps keep your dependencies up-to-date. It scans your dependency files for outdated or insecure dependencies. It then creates a PR for the dependencies that need an update. You can then review,test and finally merge dependabot's changes if you are satisfied with it. Dependabot alerts you to any outdated dependencies which can turn out to be a weakness, and if enabled, it will try to fix it by upgrading  the vulnerable dependency. If it can suggest a fix, it also sends a pull request to update your dependency manifest with the closest non-vulnerable version.
 WebD


OnlineResources
https://www.udemy.com/course/the-web-developer-bootcamp/
Force push is generally not advisable. Suppose it is a common repository with many people working on it, force pushing, when changing the history of the remote can lead to other users being out of sync and not being able to collaborate properly. It was okay for use to do it because we alone worked on our repositories.

Reordering a Commit.
If we had written all the three answers in the end, while editing the not exist commit and using the git add -p command, we would have had only one hunk to edit instead  of two, and we would have had to edit that hunk three times.

Title- Reorder the commits.

Description:

First, you have to make two commits, each containing the answer to the respective question. The title for the first commit should be "one" and that for the second commit should be "two". You can add the descriptions if you want. <br>
Ques 1 - Why would one ever need to ever reorder his commits? <br>
Ques 2 - What are Git Submodules? Why are they used?

After commiting your changes, make a PR.
Now, reorder both these commits and then again push your changes. Remember that you are not allowed to use cherry pick, squashing, reseting and reverting to reorder the commits.

NOTE: The total number of commits on the PR should be 2 only ;)
1.Create a Merge Commit: In this method, all the commits that the PR has are added to the commit history of the repository to which the PR is made, along with a merge commit which shows from which branch of which repo, the commits are merged into the repo.
2.Squash and Merge Commit: In this method, all the commits of the PR are squashed into one commit and added as a single commit to repo/branch where the PR is made.There is no extra merge commit. You also get an option to change the default commit message.
In general for this method, the repo needs to allow Squash and Merge option.
3.Rebase and Merge: In this method, the commit history is altered, i.e the commits of the PR are added individually, but without a merge commit. It can be useful in cases where a small commit needs to be added to a big project.
In general for this method, the repo needs to allow the Rebase and merge option.
4.Locally merging a commit. In this, first you have to fetch the remote into the local clone to make sure the references are updated. If the branch(B) from which the PR was created already exists, you can simply merge that into the target branch(A) using git merge B(this will not add a merge commit, the heads of A and B will be same, and the PR will close automatically.) If you merge B using git merge --no-ff, then a merge commit will also be added. 
GitSubmodules basically allows you to keep one repository as the sub-repository of another repository.It is very useful if one wants to incorporate a specific feature,code or commit from another repository,hence you won't have to use external packagement systems in which it is a hassle to manage installations.
Ques - 3 Does the merge conflicts come when you applied your stashes? Why/Why not?
Merge conflicts will arise because i have written the question 3 and the answer to question 1 in the same line.
Fetch before a pull or a merge is used to review changes being made to the local clone before they are incorporated. When one directly pulls, an attempt is made to automatically merge those changes and hence once can't review those changes. But if one uses fetch, he gets a chance to check those changes before merging them into the local clone.


The 3-stage architecture of github comprises of three stages :- Working Directory, Staging Area and the Git Directory which is the repository. How this works is that one makes some changes to files in his Working Directory, he then adds those files to the Staging Area to be committed which are then pushed to the Git Directory.
The main advantage of having the three stages, or the extra added Staging Area is that it allows you to push specific files to the staging area which can then be committed. This allows you to make different commits at the same time. For example, if one is working on two features simultaneously and he didn't have the staging area, he would have had to push the files for both the fetaures in a single commit. The Git history is not clear in such a case, but more importantly, if a bug was found and a commit had to be reverted, then the changes to all the files would have to be reverted. However, if we make two separate commits for the two different features using the Staging Area, this problem will be solved and the git history will also be improved. Another advantage of the staging area can be that the files that are added to the staging area can be pulled down as well if the need to change some code in those files is felt.

One should always fork a repository, then clone the forked repository, if he wants to contribute and is not a collaborator on the original repo. If he is a collaborator, one can make changes,  then push those changes and get them merged. However, if one is not, his/hers pushed changes will get rejected directly. However he can push those changes to his forked repository, and make a pull request from there. One is also free to experiment and make a lot of changes in the forked repository and see if pushing them works, because if you push directly to the cloned original repository, you will have to undo them.

Yes we can do that using git reflog. Git keeps tracks of all the updates in refernces. We can simply use the command git reflog to list those updates. Then we use git reset followed by the commit id of the commit to which we wanna reset to get back all the changes that were undone by git reset --hard.
The 3-stage architecture of github comprises of three stages :- Working Directory, Staging Area and the Git Directory which is the repository. How this works is that one makes some changes to files in his Working Directory, he then adds those files to the Staging Area to be committed which are then pushed to the Git Directory.
The main advantage of having the three stages, or the extra added Staging Area is that it allows you to push specific files to the staging area which can then be committed. This allows you to make different commits at the same time. For example, if one is working on two features simultaneously and he didn't have the staging area, he would have had to push the files for both the fetaures in a single commit. The Git history is not clear in such a case, but more importantly, if a bug was found and a commit had to be reverted, then the changes to all the files would have to be reverted. However, if we make two separate commits for the two different features using the Staging Area, this problem will be solved and the git history will also be improved. Another advantage of the staging area can be that the files that are added to the staging area can be pulled down as well if the need to change some code in those files is felt.