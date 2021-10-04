Hey! 👋 <br>
This is Sathwik Kuppam. <br>
I am a 2nd Year student at IIITA . <br>
To know more about me <a href = "https://github.com/Ksathwik03">visit here</a>.<br>
My created repositry is here <a href = "https://github.com/Ksathwik03/go-git"></a>

**Ques - ** You will see that some repo on GitHub has a main branch as their main but some have a master branch as their main branch. So, please explain in which case Git/GitHub creates main as the main branch and in which case it creates master as the main branch.


**Solution - **
Initializing a repo with no contents in it -
git init
git add .
git commit -m "my commit"

Now our default branch is master.

git remote add origin my_repository
git push -u origin master


Let's say we initially decide when you create the GitHub repo that you want it to have initial contents. 
Suppose we elect to start your GitHub repo with a Readme. Okay, so now the GitHub repo does have an initial branch, and it is main.

Hence github consists of 2 different main branches master and main.