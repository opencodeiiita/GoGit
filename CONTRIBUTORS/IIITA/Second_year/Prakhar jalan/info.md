.Hey!
This is Prakhar Jalan.
my profile link : https://github.com/jalanprakhar

SSH keys basically helps us to keep our data secure.If my git gets hacked the hackers would at max get my SSHkeys and not access to commit in my repos directly!
It’s primary purpose is to secure remote private transactions over the internet by providing authentication on both the server-side and the client-side in order to establish an encrypted channel between both communicating parties. 
How to edit commit message:-
1)If the commit has not been pushed:-
 you can amend the commit message with the git commit --amend command.

2)If the commit is pushed:Follow the above steps and use -push --force-with-lease


This is a vague commit!

get the commit id from git log
$ git rebase -i <commitId>
This will open an editor and show a list of all commits since the commit we want to get rid of:

1: 
2: 
3: 
pick <commitId>
pick <commitId1>
...
remove the line with the offending commit, (vi: delete current line = dd). Save and close the editor (vi: press :wq and return).

$ git push --force