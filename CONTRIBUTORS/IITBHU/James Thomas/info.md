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

**Ques** - How to edit the last commit message in git?

**Ans** - To edit the last commit the user has made, use this command <br />
git commit --amend -m "title" -m "description" . <br />
You can also write the commit message in vi editor using amend command.
However using this command makes a new commit hash, so one need to force push it to be reflected in remote repo.

### Ques - Explain the whole process that you will be using to delete that commit.

### Ans - Deleting the second commit.

After pushing the two commits, git reset to the commit hash of the correct commit(in my case first commit), now the changes will be in the working directory but the wrong commit is removed in git log

Now git stash to remove the changes in working directory also.
Git push -f and git stash drop
