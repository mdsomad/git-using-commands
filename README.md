# Git Using Commands

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Git Using Command or Install

- 👇 Windows Git Download Link
- [Git Download Website Link](https://www.git-scm.com/download/win)

<br/>
<br/>
<br/>

## Ubuntu Git installation Commands

- [Digital Ocean Git installation in ubuntu documentation Link check](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-20-04)

- 👇 Yah command se system mein agar git install hai to version check kar sakte hain

```sh
git --version
```

- 👇 Agar output same Aa Raha hai to Aapka system mein git pahle se install hai

```sh
Output  👇

git version 2.25.1

```

- 👇 yah command package ko update karne ke liye kam Aata Hai

```sh
sudo apt update
```

- 👇 yah command se git Install kar sakte hain system mein

```sh
sudo apt install git
```

- 👇 Verify the version of Git currently installed on the Ununtu machine & server

```sh
git --version
```

```sh
# Output
git version 2.26.2
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

### 👇 Git config & Configure Commands

First Stap git install ke bad
Open git bash type this commands
<br/>

- 👇 Git Mein User name add karne ka command Yah hai

```sh
git config --global user.name ""
```

<br/>

- 👇 Git Mein User email add karne ka command Yah hai

```sh
git config --global user.email ""
```

<br/>

- 👇 Git Mein User name or User email add Hua kya Nahin check karne ke liye yah command hai

```sh
git config --list
```
```sh
# Output
user.name=Your Name
user.email=youremail@domain.com
...
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

- 👇 Yah command present director Mein pahunch Chahta Hai

```sh
pwd
```

<br/>

- 👇 Yah command porject ka git ke Hawale karta hai

```sh
git init
```

<br/>

- 👇 Git Status Check

```sh
git status
```

<br/>

- 👇 Git Mini Status check

```sh
git status -s
```

<br/>

- 👇 git file ko add karta hai

```sh
git add --a
```

<br/>

- 👇 Upar wala hi Jaisa same kaam karta hai Example this is --> git add --a

```sh
git add .
```

<br/>

- 👇 Yah hai Commit kar sakta hai this is command

```sh
git commit -m "Message type"
```

<br/>

- 👇 Iska kaam hai commit History Dikhta hai

```sh
git log
```

<br/>

- 👇 Iska kaam hai commit History Dikhta hai

```sh
git log
```

<br/>

- 👇 iska kaam hai (commit) filter karka dekh sakte hai (Example jaise ke 1 3 4 )

```sh
git log -p -1
```

<br/>

- 👇 Yah hai Terminal Clear karne ka command

```sh
clear
```

<br/>

- 👇 Iska kaam hai github ka project clone karta hai This is command

```sh
git clone (url paste)
```

<br/>

- 👇 Present directory ka file show karta hai This is command

```sh
ls
```

<br/>

- 👇 Iska kaam hai Hidden File show karta hai This is command

```sh
ls -lart
```

<br/>

- 👇 Yah command edit Kiya Hua code Ko dikhana hai

```sh
git diff
```

<br/>

- 👇 Iska kaam last commit sa comper & match code changes code Ko dikhana hai this is command

```sh
git diff --staged
```

<br/>

- 👇 New Folder Create This is command

```sh
touch somad.html
```

<br/>

- 👇 Code ko changes recover karna ka kam aata hai This is command

```sh
git checkout -f
```

<br/>

- 👇 Iska kam hai only staging area se piche la jata hai Tah hai File name--> text.html (galti se add kar diya to) This is command

```sh
git rm --cached text.html
```

<br/>

- 👇 Upar wala hi Jaisa same kam karta hai (galti se add kar diya to) This is command

```sh
git restore --staged (Enter file name)
```

<br/>

- 👇 File ko complete deleted karta hai This is command

```sh
git rm Enter File name
```

<br/>

- 👇 New branch Create Kar sakta hai This is command

```sh
git branch Enter name
```

<br/>

- 👇 Branch Change & Switched Kar sakta hai This is command

```sh
git checkout Enter Branch Name
```

<br/>

- 👇 Iska kaam hai Master Branch ka Other Branch Se Marge karta hai This is command

```sh
1. yah sirf Master Branch Mein hi Kam Karega
git merge Enter Branch Name
```

<br/>

- 👇 Iska kaam hai Branch Create karne ke sath or switch bhi kar deta hai This is command

```sh
git checkout -b Enter Create Branch name
```

<br/>

- 👇Yah Command hai Branch ko deletd karta hai

```sh
git checkout -b Enter Create Branch name
```

<br/>

- 👇Yah Command File ko Rename karta hai

```sh
git mv Enter file current name Enter New Name
```

<br/>

- 👇 Yah Command File ko Delete Karta hai

```sh
git rm Enter File Name
```

<br/>

- 👇 Yah Command git Branch ko Rename & NameChange Karta hai

```sh
1. First yah karna hai
git branch -m Enter old Name Then Enter New Name
```

<br/>

- 👇 Yah command GitHub Account Remote Repository Mein New Branch Name Ka Sath Upload & push Karta hai

```sh
2. Second yah karna hai
git push origin :Enter Old Name Then Enter New Name
```

<br/>

- 👇 Yah command GitHub Account Mein push & Export Karta hai

```sh
git push origin master
```

<br/>

- 👇 Yah command GitHub Account Mein pull & Import Karta hai

```sh
git pull origin master
```

<br/>

- 👇 Yah Hai Git ko update karne ka command

```sh
git update-git-for-windows
```

<br/>

- 👇 Yah Windows ka Command hai New Folder Create karta hai

```sh
MD Enter File.Nmae
```
