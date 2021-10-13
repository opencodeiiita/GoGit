Hey!! My name is Shubhi...
Github profile link: https://github.com/Shubhi2002

Ques - What do you really understand from SSH keys? What are the advantages of using it?

SSH keys helps us to avoid writing username and password every single time when you push any change to github and authenticate it.
SSH keys are generated in pairs, a public key and a private key.
Public keys are the one that gets shared and a private key is the one that is stored only on your computer. If the keys match, you're granted access.
Basicaaly it is not only convenient but is also more secure.

Ques - How to edit the last commit message in git?

First of all you can check your current commit message by "git log"
Than to edit the messege use "git commit --amend"
This will open your vim where you can change your commit messege by pressing i(for inserting) and when done just press "Esc" and type ":wq" and press "Enter" to return back
Now you can again use the command "git log" to see the changes in commit messege.
