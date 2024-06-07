## Ubuntu Node js installation & Version list show Commands

### Commands Started

- [Node JS official documentation install Link](https://snapcraft.io/node)
- [nvm install documentation Link check](https://github.com/nvm-sh/nvm?tab=readme-ov-file)

### First install curl 👇 copy then run terminal

```sh
# 👇 curl install karne ke liye yah dono ka koi bhi command use kar sakte hain

sudo apt install curl

sudo snap install curl
```

### 👇 nvm  Installing
```sh
# 👇 copy then run terminal

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

nvm allows you to quickly install and use different versions of node via the command line.

Aapako command line ke maadhyam se node ke vibhinn sanskaranon ko turant sthaapit karane aur upayog karane kee anumati deta hai.

### Example:

```sh
$ nvm use 16
Now using node v16.9.1 (npm v7.21.1)
$ node -v
v16.9.1
$ nvm use 14
Now using node v14.18.0 (npm v6.14.15)
$ node -v
v14.18.0
$ nvm install 12
Now using node v12.22.6 (npm v6.14.5)
$ node -v
v12.22.6
```

- 1 👇 Current Selected version show

```sh
nvm ls
```

- 2 👇 Yah Command All Version List Show karta hai Node ka

```sh
nvm list-remote
```

- 3 👇 Yah Command Node Ka New Version install karta hai

```sh
# Example Yah hai --> nvm install v16.20.2

nvm install your_choice_version_add

```

- 4 👇 Yah Command Sa Check kar sakte hain Node ka Current Version ko

```sh
node --version
```

- 5 👇 Yah Command se install Kiya Hua Node Versions Sab Ko change & Switch kar sakte hain

```sh
# Example Yah hai --> nvm use v18.20.2

nvm use your_choice_version_add

```

- 6 👇 Yah command se Agar system Mein multiple node.js ka version hai to selected version ko default set kar sakte hain

```sh
# Example yha hai --> $ nvm alias default 16.14.2

nvm alias default your_choice_version_add

```

### Commands End
