## Issue #223

#### My SSH Public Key
```
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAICgTSTkhI8sx7ajnUyFD6UpJv0LD+SHIi5mhFr6mCyo8 agrawalvasu.anirudh@gmail.com

```

#### What do you understand from SSH Keys? What are the advantages of using it?
I have understood that ssh is a method to mathematically make 2 keys, one public and the other private. the private key is used to access data and public key to verify it. The benefit of this would be that it is safer than password as anyone needs both, your account and the private key to access it. So, if an account ever has to be hacked, the hacker, during a password only scenario, would ned access of only github. but in a ssh key scenario, he would need both, github and your private key, ehich is stored on your pc. so, it makes it far safer and more reliable