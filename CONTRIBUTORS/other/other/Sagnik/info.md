## Issue #223

#### My SSH Public Key
```
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDP9aXzc12Zwp9iDJm79nnHGUuegncuh+66c6/w4/yzK87ccjZZFhDyS97GP2UlSUoagLojWNpMTsa4yu6ppfIgZsZpFuPwsu2Dp7vh9eRYXrN81mu4DvLEo3O+43dqLMVoR2UCyPCK1MVAKtK1cpLTfR44SE/dSpzH6uoyQ80HhR1CsXMd1Fz1w0O/WjLnt58YzbYnzmJOjNqTnplic6a2JJDKBh61zMKE0FCSoebaTuFqDC7DoltJfvnNknP1GZiZwpX/K73fA13glTPcLwssOt7j+hMQQhH1fkKG8Zp8Swpc86pyq/jYaX7XhfmmUY39llEHuZsQmMpyP1/LC4z7uS4ijN15AUhX4j9Ezy80JxBVDhe8fHzGWDOzFb2/yaf0in5P9GjQI3Xom4Dv3GCpN3KxLGrDe9CPnAoNFzvf6meMzo3VxdqzXZ8vwSIr9bUF2kjxhwtySiM7MSg/OxrUeGW9NgT+6F9zcriLSeU8GwjjucGucxM+HAuEr1ItDyTItUwajoYg24grVoU68ACkrwtlC9iVMBPp/E/6hsKkFxbF+8G9j9bUBy1QmI2B30+J+tM/NzjFtDG0OjvPO5JF2upssM6KbmSH2X0vRASztxPE+SAVJ5BC4TRCJaGmxeHjoqYCZOtoffaxzfUDBO1rd+/JeVxYo18uU0Zwc2NSGw== SSH Key
```

#### What do you understand from SSH Keys? What are the advantages of using it?
- Uses Public-Private Key cryptography, basically two keys are made using a mathematical function, private key used for decrytion/signing while the public key, which is announced publically, and is used for encryption/verifying. This way of encryption ensures private keys never need to leave the user's device.
- Lets say in a hypothetical scenario Bob uses Basic Password Authentication, while Alice uses SSH Keys. If github were ever to be get hacked:
a. Bob's Password safety would rest entirely on githubs hand. He has to worry if they, encypted the message using modern algorthms,properly salted the passwords, how their encrytion keys were stored etc.
b. On the other hand, Alice had provided github with her ssh public key(which she has no problem with making publically available, due to the nature of public/private keypairs). And considering someone cannot forge messages using public keys, only _verify_ them. She has nothing to worry about.
Note: Bruteforcing has not been taken into consideration, however all aspects of the security provided by public/private keypairs depends on how the person secures their private keys.

- Works well with keyrings, password managers, or any other way user desires.
