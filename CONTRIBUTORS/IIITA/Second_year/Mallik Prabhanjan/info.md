Hey <br>
I am Mallik Prabhanjan <br>
This is my <a href = "https://github.com/vemulapandu">Github</a> profile <br>
This is my <a href = "https://github.com/vemulapandu/GoGit-Mallik">repo</a>

Ques - What do you really understand from SSH keys? What are the advantages of using it? (Issue: 223)

Ans) SSH key is another way to indentify ourself instead of username and password. 
     SSH keys come in pair, containing public key and private key.
     The private key remains with the user and the private key can be shared with services (eg: Github).
     For example, when you are trying to clone a repository from github, the keys are checked, and when
     they match, access is granted.
     Advantages:
        SSH keys are more secure than username and password.
        Easily identify yourself instead of typing username and password.

Ques - How to edit the last commit message in git? (Issue: 332)

Ans) In git, last commit can be edited by using the command git commit --amend. After this command, a editor 
open up in which we can edit our commit. After editing and exiting the editor, the commit is edited. 

Ques - (Issue: 336)

Ans) First I answered the ques and made the first commit. Then I added a new line and made second commit.
Then I pushed the changes and made PR. Then using git rebase -i HEAD~1 i deleted the second commit. Since
I deleted the second commit, there will be no merge conflicts. Then I force pushed this changes.
