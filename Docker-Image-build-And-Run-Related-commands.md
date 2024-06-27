### Image 🖼️ build Related commands

- 👇 Yah command se docker Image 🖼️ build kar sakte hain

```sh
# yah command mein image ka custom name Aasan Nahin kar sakte

docker build .
```

<br/>

- 👇 Yah command se doctor ka image 🖼️ build karne ke sath Custom name bhi assign kar sakte hain

```sh
docker build -t my-img .
```

<br/>

- 👇 Yah Command sa Custom name And tag breaking add Aur build & Create kar sakte hain

```sh
# Example --> docker build -t mywebapp:01 .

docker build -t custom_name_enter:01 .
```

<br/>

- 👇 Yah command se docker ka ALL Images ka list dekh 👀 sakte hain

```sh
docker image ls
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

## Docker Images 🖼️ And Container 📦 Run 🚀 Related Commands

- 👇 Yah command se docker ka image ko run kar sakte hain

```sh
# yah command Mein Ek issue hai yah Application Container ke Andar hi accessible Hota Hai Bahar Mein accessible Nahin Hota Hai

docker run image_id
```

<br/>

- 👇 Yah command se Container 📦 ko Run karne ke sath application ko container ke bahar bhi access kar sakte hain yah basically port binding hai

```sh
docker run -p 3000:3000 image_id
```

<br/>

- 👇 Yah command se Docker Container 📦 ko run karne ke sath hi Terminal </> ko free kar deta hai dusra kam karne ke liye

```sh
docker run -d -p 3000:3000 image_id
```

<br/>

- 👇 Yah Command se Container 📦 ko Run to Karega lekin Stop 🚫 karne ke sath hi Container 📦 ko remove 🗑️ ❌ bhi kar dega

```sh
docker run -d --rm -p 3000:3000 image_id
```

<br/>

- 👇 Yah Command se Container 📦 ko Run 🚀 karne ke sath hi Aap khud ka Custom name bhi assign kar sakte hain Container ko

```sh
docker run -d --rm --name "Custom name assign" -p 3000:3000 image_id
```


<br/>

- 👇 Yah command se Docker Container 📦 ko Stop 🚫 kar sakte hain

```sh
docker stop NAMES_ENTER

# Example This ---> docker stop wizardly_raman
```

<br/>

- 👇 Yah Command se Stop 🚫 & Existing Container 📦 ko Run 🚀 kar sakte hain

```sh
docker start -ai container_name
```



<br/>
<br/>
<br/>
<br/>
<br/>

## Images 🖼️ tags Related Run 🚀 Commands

- 👇 Yah Command sa image 🖼️ ko Remove 🗑️ ❌ kar sakte hain

```sh
# Example This --> docker rmi mywebapp:02

docker rmi image_name:tag
```

<br/>

- 👇 Yah command se tag Diya Hua image 🖼️ ko Run 🚀 kar sakte hain

```sh
# Example This --> docker run -d --rm --name "mywebapp02" -p 3001:3000 mywebapp:02
docker run -d --rm --name "Name_Enter" -p 3001:3000 image_name:tag
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


## Container 📦 Running 🚀 and Stop🚫 related Check 👀 Commands


- 👇 Process status yah command se docker ka Running 🚀 Container📦 check & dekh 👀 sakte hain

```sh
docker ps
```

- 👇 Yah Command se background ka Running 🚀 And stop 🚫 & Exist
  Container 📦 ka All list dekh 👀 sakte hain details ke sath

```sh
docker ps -a
```
<br/>

- 👇 Yah Command se Docker Container 📦 ko Remove 🗑️ ❌ kar sakte hain

```sh
docker rm NAMES_ENTER
```

<br/>

- 👇 Yah Command se ALL Docker Containers 📦 ko Remove 🗑️ ❌ kar sakte hain

```sh
sudo docker rm -f $(sudo docker ps -a -q)
```

<br/>

- 👇 Yah Command se ALL Docker Images 📦 ko Remove 🗑️ ❌ kar sakte hain

```sh
sudo docker image remove -f $(sudo docker images -a -q)
```
