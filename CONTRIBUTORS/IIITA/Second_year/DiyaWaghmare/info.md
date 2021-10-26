1. Merge conflicts arise when there are two different changes on the same line or same section of code so Git can't tell which chnages to include and which to remove.

Hey, my name is Diya Waghmare. 
I am a developer and student of IIIT Allahabad. 
My Github profile link is: https://github.com/diyawaghmare 
Online courses: https://sapient.udemy.com/course/the-complete-web-development-bootcamp/learn/
SSH keys are helpful so you don't have to write your username and password everytime you push to github and authenticate it. The randomly generated SSH key also makes it harder to hack and is safer to use. This is because there exists both a public and a private key, which should be stored safely by the user. It is a convenient and secure method.

Method to amend the last commit:
Type git commit --amend (If you want to open the editor and type new commit msg by entering insert mode)
or else Type git commit --amend -m "New commit msg" 
Web Development
Method to delete last commit
git reset commitid^ --hard (Reset the branch to the particular commit)
git push origin -f (Force push it to remote repository)

2. Force pushing is not a good practice because it may cause conflicts for others working in that repository and it may overwrite someone else's commit. When we did it was fine because we were the only ones working on our repositories.

3. git bisect, git hooks, git submodules

If we had added all 3 answers at the end we would have only one hunk to edit while adding commits intsead of two hunks.