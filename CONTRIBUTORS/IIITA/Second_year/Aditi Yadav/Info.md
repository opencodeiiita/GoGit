## Hey there! 👋 <br>
### This is Aditi Yadav. <br>
To know more about me, you can visit my GitHub <a href = "https://github.com/adtoria">here</a>. <br>
Visit my OpenCode IIITA '21 GoGit repository at this <a href = "https://github.com/adtoria/GoGit-Aditi.git">link</a>.

### Issue 223: <br>
#### What do you really understand from SSH keys? What are the advantages of using it? <br>
SSH Keys are <br>
- authentication credentials that manage the connection between local and remote systems. 
- like passwords, but more secure & don't require you to enter your username and password everytime.
- come in pairs of a private key and a public key.
For instance, my GitHub SSH Keys secure the connection between my local systems and my GitHub (remote).

### Issue 332:
#### How to edit the last commit message in git?
- The last commit message in git can be edited by using the command <br>
#### git commit --amend -m "correct message" -m "correct description"
<<<<<<< HEAD
=======

### Issue 366:
#### this is the second commit. i'll retain this one.
- i'll make two commits, push the changes and make a pr
- after that i'll use the command "git rebase -i HEAD~2" to see my last two commits
- in front of the first commit, which i want to delete, i'll replace the "pick" with "drop"
- in this way i'll delete the first commit and push the changes again
>>>>>>> 7de3db4 (second commit)
