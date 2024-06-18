# Git

### Local Config
```
git config user.email "kiros33@gmail.com"
git config user.name "Sangyong Bae"
```

### ssh 생성
```
➜ .ssh  ssh-keygen
Generating public/private rsa key pair.
Enter file in which to save the key (C:\Users\kiros33/.ssh/id_rsa): id_rsa_kiros33
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in id_rsa_kiros33.
```

### Key 지정 및 Clone
* Git Bash
```
GIT_SSH_COMMAND="ssh -i ~/.ssh/id_rsa_kiros33 -o IdentitiesOnly=yes" git clone git@github.com:kiros33/flutter-study.git
```
* Powershell
```
$env:GIT_SSH_COMMAND="ssh -i ~/.ssh/id_rsa_kiros33 -o IdentitiesOnly=yes"
git clone git@github.com:kiros33/flutter-study.git
```



