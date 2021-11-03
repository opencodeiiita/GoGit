This is Shashwat Mittal
Student at IIIT Allahabad.
Sophomore-IT
repo link: https://github.com/shashwat-mittal/GoGit.git

Ques- What do you really understand from SSH keys? What are the advantages of using it?
SSH keys are used for authentication. They help to connect to github without without using your password or credentials any time. 
It grants access to multiple users without sharing the password. It acts as a convenient way of authentication.
It consists of a public and private key where the private key stored in the system is never revealed to server or any other user.

Ques - What is a GitHub gpg key? Why it is used? Also, tell that why we need to sign the commits?
It is a public key used by the github to verify signatures. 
When we sign a commit with our private gpg key and submit the modifications to github, github verifies the signature using the public gpg key, and we obtain a verified commit.
It helps to verify the identity of the commiter.

Ques 2 - What are Git Submodules? Why are they used?
ans : git submodules is a record in our repository which is pointing to a specific commit in some other repository. In some cases, where the external repository changes very frequently, incorporating changes may become difficult and could also break our application or api. Thats why we use git submodules to point to a specific commit and lock its code at a particular commit.

Ques 1 - Why would one ever need to ever reorder his commits?
ans : sometimes a particular order of commits make more sense. It may used when we need to push only one commit to the remote.

 
