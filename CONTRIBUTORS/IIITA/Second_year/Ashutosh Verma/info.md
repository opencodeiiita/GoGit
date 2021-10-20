## Que1(issue-409) How and why merge conflicts arise? 
## Ans:
Merge conflict arises when two branches diverge from each other and in both branches changes are made in the same line of the same file. So, git is not able to decide how to arrange both changes.It also occurs if there is a difference of any new line character
## Hey👋 Everyone!!
This is Ashutosh Verma. <br>
This is my GoGit Repo. I'm a second year student at IIIT-A.
To know more about me, you can visit my GitHub <a href = "https://github.com/ashutosh3027">here</a>. <br>
Link of my repo, <a href="https://github.com/ashutosh3027/first-time-Go_git"></a>

## Que(issue-10):
Create a directory inside CONTRIBUTORS of any name. <br>
Now add, commit and push your changes to the repo.<br>
So simple, just do that.<br>
⌚
⌚
But in doing so you will face a problem.
I want that problem (you faced above) and the reason for that problem i.e. why you are facing that problem inside your info.md file.

## Ans:
The problem is after creating an empty directory in CONTRIBUTORS whenever I was trying to track that same empty folder through git status commands not able to track it not even able to push it to remote repository.

The reason for the same problem is that git doesn't include them in commits and it certainly doesn't include an empty directory when we push to GitHub.


## Que(issue-223):
What do you really understand from SSH keys? What are the advantages of using it?

## Ans:

SSH is Secure Shell Protocol. It allow us to connect remote computer by using text based interface. Using ssh we can log into another compter and perform any commands on that computer securely. It provide secure connection between two host in insecure network.In terms of github, github is server side computer and aur local system is a client server. Using ssh key we make secure connection between the same host and they mainly comes in pair one is public and other one is private.


## Que(issue-332) How to edit the last commit message in git?
## Ans: 
By using commond git commit --amend and pressing enter it will open a editor in which we can first press i to enter in insert mode then you can edit last commit message.



## Que(issue-366)
## Ans:
  Firstly i have clone it in my repo then made changes in my info.md file by just writing que of this issue after that i have made a commit .Then, In seoncd commit  the whole process by which I will delete my first commit is explained. After making two commits I will use git rebase -i Head~2 then a editor will open there I will use drop insted of pick for that commit which I want to discard in my case it is first commit. That's it.

## Que2(issue-409)  Is force push a good practice? Yes/No why? In most of the tasks on this repo, you used force push, so why this practice is Okay (neither good nor bad) in your case?
## Ans::
Force push is good or bad depending on the situation. In most tasks, we used force push in this repo because we are instructed to do tasks in 1 or 2 commits so to squash unnecessary commit and push it on GitHub we used force push. Force push is used when direct push is not possible and our commit history is not matching with remote repo commit history. But we need to keep all committed for future references.  
## Que3(issue-409) Name anyone Git or Github topic on which any issue is not made on this repo. 
## Ans:
How to add different remote repo to our own repo locally to perform fetch opteration.