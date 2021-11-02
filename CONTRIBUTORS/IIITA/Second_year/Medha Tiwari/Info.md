#### Ans 1 for issue -[409](https://github.com/opencodeiiita/GoGit/issues/409)
In my opinion, merge conflicts arise when a change in single location is done at two places at the same time. Scenarios could be two people working in the same file or a single person working on the location in diffrent branches.
<hr>

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
Answer 1> Web dev, blockchain

### Issue [332](https://github.com/opencodeiiita/GoGit/issues/332)
git commit --amend (command to edit the last commit message) this will open up a editor (vim mostly) and we can edit the message 
in the editor(i -> insert mode, write the commit message and the press'ESC' and :wq to exit)


OR

git commit --amend -m"commit message"
Answer 2> freecodecamp.org, reading docs
<hr>

#### Ans 2 for issue -[409](https://github.com/opencodeiiita/GoGit/issues/409)
As in general force push is not considered to be a good practice when several people are working on the same issues. It overwrites the commits which may result into loosing commits hence the track of the contribution.
But when we are the single person working on the issues or in a particular directory that in most case is independent (as the most of the tasks/issues in this repo), we can use it to change our commit message, squashing (after pushing it to remote) etc.
<hr>

#### Ans 3 for issue -[409](https://github.com/opencodeiiita/GoGit/issues/409)
Well, I can't think of one right now. Just for the sake of answering
refer [this](https://www.atlassian.com/git/tutorials/dotfiles)

<hr>

#### What changes to your procedure of doing this task will happen if I told you to write all first three answers (Ans - 1, 2, 3) at the end of the file.

Only change I observed was that if all the answers were written continuously then git will not consider them as separate hunks and we have to manually edit the patch two times(first for ans-1 and ans-2 and second for ans-2 and ans-3) compared to now when I have just edited that one time (for ans-2 and ans-3).


[Issue 431](https://github.com/opencodeiiita/GoGit/issues/431)
1) We use git fetch to know/review the changes before actual pull i.e. merging with our working copy. Pull automatically merge the changes with our local repository.

Ques - 3 Does the merge conflicts come when you applied your stashes? Why/Why not?
Ans. Yes because I was working on the same location for ques-1 and ques-3 
