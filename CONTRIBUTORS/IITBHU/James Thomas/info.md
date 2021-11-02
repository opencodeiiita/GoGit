### Ques-1 How and why merge conflicts arise?

**Ans-1** According to me, merge conflicts arise when two different changes on the same line occurs in a file. Eg. merging 2 branches. However git cannot solve it automatically, thus its the work of the developer to consider which changes he likes to keep.

Hey !!! <br/>
James this side , 2nd yr student from IITBHU <br/>
My git repo <a href = "https://github.com/james3gh/go-git-jt">Link</a> <br/>
To know more, <a href = "https://github.com/james3gh">click here</a>.

**Ques** - What do you really understand from SSH keys? What are the advantages of using it ?

**Ans** - It is medium through which a local server can send/receive data to a remote server in a secure manner. SSH has a public and private key.

- Data is encrypted (specially username and password is secured)
- File transfer is much safer.
- Through SSH key it doesn't require to enter usrnme and passwrd everytime we clone our repo.

<br />
### Ques-4 What changes to your procedure of doing this task will happen if I told you to write all first three answers (Ans - 1, 2, 3) at the end of the file.

**Ans-4** If all the 3 ques were answered at the end then it will not be possible to split the hunk. However the procedure remains same using edit command.

**Ques** - How to edit the last commit message in git?

**Ans** - To edit the last commit the user has made, use this command <br />
git commit --amend -m "title" -m "description" . <br />
You can also write the commit message in vi editor using amend command.
However using this command makes a new commit hash, so one need to force push it to be reflected in remote repo.

### Ques-2 Is force push a good practice? Yes/No why? In most of the tasks on this repo, you used force push, so why this practice is Okay (neither good nor bad) in your case?

**Ans-2** Force push is not a good practice though as it changes the git commit history. The other contributors working on a project can face issue due to this.
In our case, as working on the individual named files, doesn't make any change to the files of other contributors. Moreover, in our case we as individul were working on our own repositories. The owner of the repo if force pushed the changes then all the other contributors working on the repo may loose some data.

### Ques-3 Name anyone Git or Github topic on which any issue is not made on this repo. (Your answer should be different from others.

**Ans-3** Working on some issue that uses some concept of detached head if added can be really helpful.

Git merge - It merges the two branches either by fast forward or recursive approach. No commit is made if made by ff approach. If destination branch is ahead in some commits then, an extra commit is made to merge by recursion. But git history becomes filled with lot of commits.

Git sqaush and merge - It takes all the changes but squashes all the commits into one commit. It is useful when only the changes are nessecary rather the extra commits, making commit history clean. However, no linked reference to the original commits are present in the history.

Git rebase and merge - It appends all the changes from base of feature branch and put it at the end of destination branch. It does not make any extra commit. It is useful for a plain straight git history. However, it rewrites the history.

Git merge --no-ff - It forces a merge commit, preventing a fast-forward commit. It makes an extra commit such that the destination branch is ahead of feature branch by 1 one merge commit. Through this, commit history is retained from branch being merged. It makes a detailed git history.

# Squash and Regret 🙂

## Issue_Description :

First make two commits in your info.md file each having respective answers to the questions. Commit title of each commit should be `<GitHub-username>-one` and `<GitHub-username>-two`. No commit description is required.

**Q1** - Explain objects and refs folder inside ./git. Where git commits are stored in ./git folder?

**Q2** - Differentiate between tree and blob in git? What they represent?

Then squash both the commits into one. Title of squash commit can be anything.

### NOTE: After cloning, one can use only 3 git commands uptil squashing the commits. (Even git status will get count)

Now make a `new_Branch`. Delete the squash commit from that branch.
Now recover back the changes made in the commit 1 and 2 **individually** by cherry picking. i.e. first cherry-pick the 1st commit `<GitHub-username>-one`, then cherry-pick the 2nd commit `<GitHub-username>-two` into the `new_Branch`. Solve merge-conflicts if any.

Now make a PR from this `new_Branch`.

#### NOTE: The total number of commits on the PR should be 2 only and only one PR is allowed

Ques 2 - What are Git Submodules? Why are they used?
Ans 2 - Git submodules is like a git repository inside another git repo. Changes made in submodules are not tracked by main repo. It is useful to have some separate projects inside a git repo if the projects is much complex. This make the projects divide into small modules to work upon.

Ques 1 - Why would one ever need to ever reorder his commits?
Ans 1 - Reordering commits makes a clearer and understandable git history. It makes the developer understand their code changes in a uniform and time-based manner. It also helps to push some particular commits by changing the order.

**Ques - 3 Does the merge conflicts come when you applied your stashes? Why/Why not?** <br/>
**Ans - 3** Yes merge conflict arised as the changes made by me on ques 1 and ques 3 were on the same line of the file after applying stashing .

**Ques - 1 Why do we do fetch before the merge or pull?** <br/>
**Ans - 1** Git fetch collects all the changes made in the remote repo to one's local repo. It doesn't make any local changes to your repo. Through git fetch one can see all the branches and changes made in the remote repo without disturbing your local changes. Then though git merge it changes the local changes acc. to the remote repo's changes
