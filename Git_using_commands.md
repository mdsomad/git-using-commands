### Git Using Command or Install
First Stap git install ke bad 
Open git bash type this commands
- Git Mein User name add karne ka command Yah hai
```sh
git config --global user.name ""
```
- Git Mein User email add karne ka command Yah hai
```sh
git config --global user.email ""
```
- Git Mein User name or User email add Hua kya Nahin check karne ke liye yah command hai
```sh
git config --list 
```








- Yah command present director Mein pahunch Chahta Hai
```sh
pwd
```

- Yah command porject ka git ke Hawale karta gai
```sh
git init
```


- Status Check
```sh
git status 
```

- Mine Status check
```sh
git status -s
```

- Sam kaam karta hai
```sh
git add --a
```

- Yah do Sam kaam karta hai
```sh
git add .
```

- Yah hai Commit kar sakta hai this is command
```sh
git commit -m "Message type"
```

- iska kaam hai commit History Dikhta hai
```sh
git log
```

- iska kaam hai commit History Dikhta hai
```sh
git log
```

- iska kaam hai (commit) filter karka dekh sakte hai (Example jaise ke 1 3 4 )
```sh
git log -p -1 
```

- Yah hai Terminal Clear karne ka command
```sh
clear
```

- Iska kaam hai github ka project clone karta hai   This is command
```sh
git clone (url paste)
```

- Present directory ka file show karta hai   This is command
```sh
ls
```

- Iska kaam hai Hidden File show karta gai   This is command
```sh
ls -lart
```

- Yah command edit Kiya Hua code Ko dikhana hai  
```sh
git diff
```

- Iska kaam last commit sa comper & match code changes code Ko dikhana hai   this is command
```sh
git diff --staged
```

- New Folder Create     This is command
```sh
touch somad.html
```

- code ko changes recover karna ka kam aata hai     This is command
```sh
git checkout -f
```

- Iska kam hai only staging area se piche la jata hai Tah hai File name--> text.html (galti se add kar diya to)    This is command
```sh
git rm --cached text.html
```

- Upar wala hi Jaisa same kam karta hai  (galti se add kar diya to)    This is command
```sh
git restore --staged (Enter file name)
```

- File ko complete deleted karta hai   This is command
```sh
git rm Enter File name
```

- New branch Create Kar sakta hai   This is command
```sh
git branch Enter name 
```

- Branch Change & Switched Kar sakta hai   This is command
```sh
git checkout Enter Branch Name 
```

- Iska kaan hai Master Branch ka Other Branch Se Marge karta hai  This is command
```sh
1. yah sirf Master Branch Mein hi Kam Karega
git merge Enter Branch Name 
```

- Iska kaam hai Branch Create karne ke sath or switch bhi kar deta hai    This is command
```sh
git checkout -b Enter Create Branch name
```

- Yah Command hai Branch ko deletd karta hai   
```sh
git checkout -b Enter Create Branch name
```

- Yah Command File ko Rename karta hai   
```sh
git mv Enter file current name Enter New Name
```

- Yah Command File ko Delete Karta hai   
```sh
git rm Enter File Name
```

- Yah Command git Branch ko Rename Karta hai   
```sh
git branch -m Enter old Name Then Enter New Name
```

- Yah Command git Branch ko Rename Karta hai   
```sh
git branch -m Enter old Name Then Enter New Name
```

- Yah command GitHub Account Remote Repository Mein New Branch Name Ka Sath Upload Karta hai    
```sh
git push origin :Enter Old Name Then Enter New Name
```

- Yah command GitHub Account push & Export Karta hai    
```sh
git push origin master  
```

- Yah command GitHub Account pull & Import Karta hai    
```sh
git pull origin master
```


- Yah Windows ka command hai New Folder Create karta hai    
```sh
MD Enter File.Nmae
```