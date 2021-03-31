# SSH-login-without-password
how to SSH login without password

## 4 steps todo
```
ssh-keygen -t rsa
ssh username@hostname mkdir -p .ssh
cat .ssh/id_rsa.pub | ssh username@hostname 'cat >> .ssh/authorized_keys'
shh username@hostname
```

## Depending on your version of SSH you might also have to do the following changes:
Put the public key in .ssh/authorized_keys2

Change the permissions of .ssh to 700

Change the permissions of .ssh/authorized_keys2 to 640
