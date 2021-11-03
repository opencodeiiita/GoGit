Ans1) Merge conflicts happen when people make different changes to the same line of the same file, or when one person edits a file and another person deletes the same file. And when the differences of 2 or more commits coincide then a merge conflict takes place.

Hi this is Shailesh Tiwari!
This is my profile https://github.com/shlesh

What do you really understand from SSH keys? What are the advantages of using it?

SSH keys are just plain text created using ssh-keygen, like passwords but they are more secure. Each SSH key pair includes two keys: public key that is copied to the server and private key that remains with the user.
We don't have to write your username and password everytime
ssh keys are almost impossible to hack.
I do Web Development
How to edit last commit message using git?
The git commit --amend command allows you to change the most recent commit message.

Ans2) Normally, it is not a good practice (unless you are the only one using the repo) otherwise it can cause all sorts of issues for the other collaborators. It was alright for us in opencode as we would be making separate PR's thus it wouldnt conflict, but in a general use case its not good practice.

Ans3) I dont think ` git tag` and ` git revert` havent been done yet.
AnswerFInal) If I had to add all the three answers together, then they would come as a part of just one chunk and we will then have to `edit` that chunk.



Ques - 1 Explain in detail the three-stage architecture of Git.  
Referred to [this articles](https://raghav20nov.medium.com/git-and-github-for-beginners-3-ceeb016f410b)
We work on our working directory, commit some changes, and then push to the repository in a two-stage Version Control System. Then we can pull the changes from the repository (changes made by our colleagues), commit some changes, and push the files back to the repository.
It appears to be very good up to this point, but imagine you're working on a project with, say, four files. You've finished working on two files, but you've discovered a bug in the other two. If you commit changes to the repository in this case, the other two files containing the bug will also be committed to the repository. This is a major issue!
However, git solves this problem by introducing a middle stage called "staging area" in this design. Let's have a look at three-stage architecture now. Thus, git allows us to first push our files to the staging area, and then commit those staged files. Continuing with our previous example, we can only push those two bug-free complete files to the staging area and then commit our modifications. The other two files in progress can be left in our working directory. They can be changed later and committed when necessary. Another significant benefit of the staging area is that files from the staging area can be dragged back into our working directory if we believe they require additional adjustments before being committed.
In git, it is not necessary to first push the files to the staging area. The modifications can even be committed directly, but it is usually a good habit to stage our files first.
