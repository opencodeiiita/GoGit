###Ques - 1 How and why merge conflicts arise? (Answer from your own understanding)

###Ans- Acc. to my understanding, a merge conflict happens when you merge two separate branches that contain different changes on the same locations in the same file and it's unclear which change should take precedence or whether both should be combined.


Hello, I am Dheeraj bhardwaj 2nd year student at IIITA.


Github profile : https://github.com/Dheeraj096


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
                            
                            
   ###Ques - 2 Is force push a good practice? Yes/No why? In most of the tasks on this repo, you used force push, so why this practice is Okay (neither good nor bad) in your case?

###Ans - In short according to me it is not a good practise because Force-pushing is a highly threatening and risky method if you're working in a common repository. Using this force pushing you should be able to force your local revision to the remote repository.Like if many people are working on same issue then Force modifying the git history can get your collaborators out of sync but if you alone who is working on that issue then it is ok.    
    
    
 ###Ques - 3 Name anyone Git or Github topic on which any issue is not made on this repo. (Your answer should be different from others.

###Ans - Any issue regarding gitk command.      
    
    
    
 ###Ques - What changes to your procedure of doing this task will happen if I told you to write all first three answers (Ans - 1, 2, 3) at the end of the file.
 ###Ans - no change   
