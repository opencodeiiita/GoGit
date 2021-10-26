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

#### [Issue 445](https://github.com/opencodeiiita/GoGit/issues/445)

Ques - Explain the procedure you used to solve this task. Also, explain that why this process is the best option to find out that, when and what bug got introduced in your code?
- I used git grep "This is a bug file"
- used git log to find the time and found who introduced this and when
- As this process doesn't affect any other process it is viable to use.
- Sun Oct 24 01:30:33 2021 (when) 
- (what) a file name bug.md in CONTRIBUTORS/IIITA/Second_year/Isha Rawat