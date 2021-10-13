# Hi I'm Ritwik Rajput

From Indian Institute of Information Technology Allahabad

My Github profile : "https://github.com/kaneki-ken260"


Question: What do you really understand from SSH keys? What are the advantages of using it?

Answer:  Secure Socket Shell (SSH) Key Management, is a special network protocol leveraging public-key cryptography to enable authorized users to remotely access a computer or other device via access credentials called SSH keys and without actually transmitting the password to the server.
        The advantage of using SSH keys is that we can be authenticated by the server without even entering our password. This is quite safe as even if someone tries to crack the password either by brute-force approach or by any other method, the chances are quite less because the actual password was never transmitted to the server.
        It is more convenient as if we use an SSH key with an SSH agent, we can connect to multiple servers without even entering the password for each system.

Question: How to edit last commit message in git?

Answer:  For editing our last commit message in git we have to use a command "git commit --amend", this will show us the last commit message and also the option to edit this.
         After editing our last commit message we just have to type ":wq" and we will exit the wim and thus we have our last commit message edited. 
         
Question: Explain the whole process that you will be using to delete that commit.

Answer : I will be answering this in my second commit message and deleting my first commit message. After making the second commit and pushing the commits , I just used "git rebase -i HEAD~2" in order to rebase the last two commits.
         Then I replaced the "pick" keyword before the first commit message with "d" keyword and then use :wq to exit wim and then forced push the commits using "git push --force".         
