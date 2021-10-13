### Hey, I'm Varun Tiwari
I am a student of ABV-IIITM, Gwalior.
To know more about me [visit here](https://github.com/varunKT001)
This is the link of the repo [GoGit_repo](https://github.com/varunKT001/GoGit)

## Issue : 223 
#### Ques - What do you really understand from SSH keys? What are the advantages of using it?
SSH keys are just pairs of a public and private key. The Private keys are used to encrypt/decrypt the user identity. SSH keys provide more security as well as convinience to the user.  

## Issue : 332 
#### Ques - How to edit the last commit message in git?
There are two cases : 
1. Changes not pushed : If changes are not pushed we can simply add --amend flag and it will amend last commit. 
2. Changes are pushed : If Changes are pushed we need to --amend the and also force push the changes using the -f flag

## Issue : 366
#### Ques - Explain the whole process that you will be using to delete that commit.
I will delete second commit so i write ans here. To delete a commit i will use 'reset'. using this my repo will go to previous commit state and loose all other commits. i will provide the commit hash to where i want to revert my repo to. 