Hey! 👋 <br>
This is Sathwik Kuppam. <br>
I am a 2nd Year student at IIITA . <br>
To know more about me <a href = "https://github.com/Ksathwik03">visit here</a>.<br>
My created repositry is here <a href = "https://github.com/Ksathwik03/go-git"></a>


Initializing a repo -
git init
git add .
git commit -m "my commit"

Now our default branch is master. So we have to decide now whether to keep that or change it to main.

If we decide to keep it as master, then:

git remote add origin my_repository
git push -u origin master


On the other hand if we decide to keep main branch our main branch, then:

git remote add origin my_repository
git branch -M main
git push -u origin main

Hence github consists of 2 different main branches master and main