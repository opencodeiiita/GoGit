Merge Conflicts arise when commits are added to the same place in a file, when they coincide.Suppose both the commits want to add changes to the same line, they are not overwritten by each other, and hence merge conflicts arise.
Hey!<br>
This is Raghav Goel.<br>
My  <a href = ""https://github.com/raghavgoel25"">Github Profile</a>

What do you really understand from SSH keys? What are the advantages of using it?

SSH key is a method that can be used for authentication different from normal passwords mainly in the way it operates. 
SSH keys are more long than typically used passwords and are computer generated, making them less prone to hacking. 
 They are not stored on servers, but only the device which is being used for login, hence again
making it less vulnerable to hacking.
 
 How to edit the last commit message in git?
 The following commands should be executed:-
 1.git commit --amend -m "New message" 
 2.git push --force repository-name branch-name
 If you are not sure whether someone has cloned your repository after your latest commit, instead of the second command, use.
 git push --force-with-lease repository-name branch-name
 This command will abort the push if there are any upstream changes to the repository, whereas the --force command will destroy any changes.


 How to delete a commit?
 I will use git reset --hard HEAD^ to delete the latest commit i will have made.
 
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
Explain the procedure you used to solve this task. Also, explain that why this process is the best option to find out that, when and what bug got introduced in your code?

I used git log -p to see the commit history along with the changes introduced in the commit. This opened a less window in my terminal. I then used the / command to search for a string and then searched for "bug", which led me to the commit where the bug file was added and also showed me the hash for that particular commit. I found this particular method useful here because the input of the file was given to me, and i could easily search for it using the command in the less window.
Also since the entire history of the commit along with the changes made in it is shown in git log -p, it helped me find out when the commit was made along with the problem of the bug.

