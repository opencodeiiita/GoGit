Ques - 2 Should I make some issues on GitHub workflows for some Maven and Gradle projects?
Umm, don't know much about them. But yes, make some, I'll try to learn :)

Ques - 4 If you have made only two commits for this task, then why there are only two, not three, and if there are three commits for this task then why there are three, not two?
I have two commits. 
Firstly i answered question 1 and stashed. 
Then i added question 3 in info.md and question 2 in a new file temp.md. Now since the new file is not tracked, stash won't be applied to it using command: 
git stash
To include this file also, we will use: 
git stash -u
now all the changes (including new file) will be stashed. So now I have 2 stashes. So now I applied stash with question 2 and 3, added answers to them, and then committed the changes. Then I applied the stash with answer 1, removed conflits, and committed the changes. Therefore I have 2 commits. If I had made three stashed (seperate stash for new file), there would be 3 commits (for each stash changes).
Ques - 1 Why do we do fetch before the merge or pull?
while using git pull, git takes the changes on the remote repo and tries to automatically merge them to our local copy. But if we want to review the changes first, we cannot do that with git pull. That's where we use git fetch. git fetch command searches for changes and commits on the remote (which are not on our local copy) and saves them without automatically merging. We can review the changes before we merge them. 
