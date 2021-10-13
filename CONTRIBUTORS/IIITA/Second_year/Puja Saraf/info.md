## Hello there!!!

### I am Puja Saraf.

visit my GitHub to know more about me <a href = "https://github.com/Puja-Saraf">click</a>.

While working on a repository, SSH key can be used to identify ourself without using github username and password.
When we try to log in, server checks the public key and generates a random string and encrypts it using the public key.
And it could be decrypted only with corresponding private key (which is on our computer). Now our computer decrypts it and send the message back to the server.
And for security reasons it also acts as a password so that no third party could push changes to the repo.

#### issue-366
In the first commit I'm answering the question and I'll be deleting the second commit.

Commands to delete the last commit:

git reset --hard HEAD~1

When using git reset --hard HEAD~1 we will lose all uncommited changes and all untracked files in addition to the changes introduced in the last commit.

git push -f origin main