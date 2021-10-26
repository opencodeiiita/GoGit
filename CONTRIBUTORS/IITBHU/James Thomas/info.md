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

**Q** Explain the procedure you used to solve this task. Also, explain that why this process is the best option to find out that, when and what bug got introduced in your code?

**A** First used git grep "bug" to find content in which directory/file this is found. <br/>
Then used git log -S"This is a bug file" && git log --after="2021-10-14" <br/>
This showed the author, date, time and commit hash.This is useful as it searches the git log according to the date and content of the bug/issue caused.
