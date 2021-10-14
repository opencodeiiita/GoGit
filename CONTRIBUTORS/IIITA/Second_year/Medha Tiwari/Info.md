Hey, Medha this side.
<br>
I am a sophormore at IIIT Allahabad.
- [Github](github.com/medhatiwari)

- Repo Link is [here](https://github.com/medhatiwari/fantastic-broccoli)

### Issue [223](https://github.com/opencodeiiita/GoGit/issues/223)

#### What do you really understand from SSH keys? What are the advantages of using it?


SSH is secure channel for communcation with remote. It has a key pair (Asymmetric cryptography ie, one public and a private key). Public key is stored on the server that we log into(here it is github) and the private cryptographic key is stored on our computer.



When we try to log in, server checks the public key and generates a random string and encrypts it using the public key.
And it could be decrypted only with corresponding private key (which is on our computer). Now our computer decrypts it and send the message back to the server.



Kinda, better than password authentication. why? 
SSH keys are difficult to compromised as these keys are longer in length (up to 4096 bits), that makes them hard to guess.

Not like passwords, ssh keys aren't sent to the server, So even hackers exploit the server they can't access our accounts. 


### Issue [332](https://github.com/opencodeiiita/GoGit/issues/332)
git commit --amend (command to edit the last commit message) this will open up a editor (vim mostly) and we can edit the message 
in the editor(i -> insert mode, write the commit message and the press'ESC' and :wq to exit)


OR

git commit --amend -m"commit message"


### Issue [366](https://github.com/opencodeiiita/GoGit/issues/366)

For deleting the commits I have used git rebase -i (interactive rebasing).

Lets say I have made two commits "commit-1" and "commit-2" (in that order) and I have to keep one of them and delete (or drop) the another one.

for this I will use the sha key of the commit that was made before these two commits.

Now, this will open up the editor for me with two commits on the top of the editor, now I can just remove one of them and woala I have deleted the commit.(easy peasy ;))

Since my last [Pr](https://github.com/opencodeiiita/GoGit/pull/384) didn't get merge

So here I am to give it a another try

In this I will first make two commits as above but this time I will not use rebasing instead I will use revert (which is going to make one more commit i.e, a revert commit) and then I will squash them into one (for which I will use interactive rebasing).

(Ultimately doing interactive rebasing) I am just doing revert to make it a different method :(