# Table of Contents
```
notes:

Several Contents are based on Pro git book,
Thanks for all the contributors of the book

this guides is performed in linux environment
```
to get the book:
https://git-scm.com/book

1. Installing Git
2. Setup Git Config
3. Playing with git
4. Adding SSH Key to github

## Installing Git
```
sudo apt install git-all

to check our installation, run:
git --version
```

## Setup Git Config
```
To view all your settings, run:
git config --list

To set username and email address, run:
git config --global user.name "<your_username>"
git config --global user.email "<your_email>"
```

## Playing with git
```
1. To create git repository, run:
git init

2.  Perform the versioning, run:
git add <everthing_you_want_to_track>
git commit -m <message_you_want_to_write>

ex:
git add file.txt
git commit -m "Add file"

3. Clone an existing repository (ex: Github), run:
git clone <URL>
ex:
git clone https://github.com/Giffari17/Devops-Learning.git (using https)
git clone git@github.com:Giffari17/Devops-Learning.git (using ssh)

note:
if you want to clone using ssh setup the ssh key first
```

## Adding SSH Key to github
```
1. Open the terminal

2. To generate public and private key, run:
ssh-keygen -t rsa -b 4096 (RSA Algoritm)
OR
ssh-keygen -t ed25519 (ED25519 Algoritm)

3. To find your generated keys:
cd ~/.ssh
ls

4. Get the public key to be stored at github:
cat ~/.ssh/id_ed25519.pub

5. Copy the output

6. Go to your github settings, SSH and GPG keys

7. New SSH Key, fill every field (put the "key type" as default), paste your public key to "key" field, Add SSH Key

8. If adding key has run successfully, now you can perform "git clone" using SSH
```