
  Q:-What type of development I do?
  Ans:- Web development and cc. 



Heyy! 

This is me Dheeraj bhardwaj.

To know more about me visit here :- https://github.com/Dheeraj096/First_time01.git 

Github profile:- https://github.com/Dheeraj096


Ques - What do you really understand from SSH keys? What are the advantages of using it?


Ans  - Basically from my understanding SSH keys are secure alternate to email and password like we don't have to write everytime email and password for authentication. SSH key  is automated for implementing single sign-on system method. It comes in pairs <public and private>  public key -  sharing with github. private key - stays on local machine. As when both keys matches we are allowed to make changes.

  Advantage:-
  
  SSH keys are much securer and easier because we don't have to write anything email and password. Also there is no chance of spelling mistake.
  
  It easily identify yourself no one can identify our private informations like password.
  
  Answering issue of #366
  Ans:- After making two commits and making PR
  Checking branch with git checkout -b my_branch_with_extra_commits
  then opens git console using gitk
  then look for the commit that we want to keep  and copy the SHA of that commit.
  then git checkout my_branch
  then gitk
  then right click on the commit we want to revert
  then do a git pull --rebase origin branch_name_to_merge_to
  then git cherry-pick <SHA we copied earlier
                            

  Q:- Resources that I follow?
                            
  Ans:- Youtube , technical blogs, w3school, geekforgeeks etc.                          
  
  Ways of merging
  1)) creating a merge commit :- This is a straight forward method it merges all commits from pr and also create a one more commit of merge commit in which details of merge in our master branch.  
                            
  2)) Squash and merge :- So this ia a second method of merging pr. If in your pr there are so many commits then it squash it to a single commit and then merge the changes in remote repositiory.
                            
  3)) Rebase and merge :- Now this is the third method of merging pr by rebasing. This method modifies the git commit history. There is no extra Merge commit. Like if we want to merge pr in main branch from test branch then by rebasing and mrging method the recent commit of the pr will becomes the HEAD of our main branch.
                            
  4)) Through local terminal:- Ex. I have to merge in main-copy branch from my  waste5 branch 
                            
command followed:-git checkout main-copy
                            
git pull origin main-copy
                            
git fetch origin
                            
git checkout waste5
                            
git merge main-copy
                            
git checkout main-copy
                            
git merge --no-ff waste5
                            
git push origin main-copy
                            
                            
                            
                            
