##Hey! <br>
This is Agrim Verma. <br>
My <a href="https://github.com/AgrimVerma">Github profile</a>

What do you really understand from SSH keys? What are the advantages of using it?

SSH keys are just plain text created using ssh-keygen, like passwords but they are more secure. Each SSH key pair includes two keys: public key that is copiedto the server and private key that remains with the user.
- You don't have to write your username and password everytime
- ssh keys are difficult to hack as these are very long.

How to edit the last commit message in git?
We use following commands:
git commit --amend -m "New commit message"
If already pushed commit to the remote branch, then - after amending our commit locally we also need to force push the commit with:
git push <remote> <branch> --force
