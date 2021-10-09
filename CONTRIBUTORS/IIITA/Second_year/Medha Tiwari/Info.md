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