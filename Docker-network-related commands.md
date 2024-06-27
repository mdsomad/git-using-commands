# Docker Network Related Commands

<br/>
<br/>


- 👇 Yah command Se Khud 👨🏻‍💻 ka custom network 📶ᯤ create kar sakte hain

```bash
# Example --> docker network create -d bridge my-custom-network

docker network create -d bridge network_name
```

<br/>

- 👇 Yah command se Check & Dhkh 👀 kar sakte hain kaun kaun sa network📶ᯤ available hai

```bash
docker network ls 
```

<br/>

- 👇 Yah command Container 📦 ko host🖥️ network📶ᯤ Mein Run kar sakte hain

```bash
docker run -it --network=host busybox 
```

<br/>

- 👇 Agar Container 📦 ko 🚫📵 none network📶ᯤ Mein connect ho to usko internet ka access Nahi milega

```bash
docker run -it --network=none busybox
```

<br/>

- 👇 Yah command se  Check & Dhkh 👀 kar sakte hain kaun kaun sa Container 📦Bridge network ᯤ 📶 se connected hai

```bash
docker network inspect bridge
```

<br/>

- 👇 Yah Command se Create Kiya Hua Network ᯤ 📶 ko Remove 🗑️❌ kar sakte hain

```bash
# Example --> docker network rm my-custom-network

docker network rm custom-network_name
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>


- 👇 Is Tarike Se Alag Alag Container 📦 ko ek hi network 📶ᯤ ke sath RUN kar sakte hain

```bash
docker run -it --network=my-custom-network --name container1 ubuntu

docker run -it --network=my-custom-network --name container2 busybox

ping container1
```
<br/>

- 👇 Yah command se check kar sakte hain is network 📶ᯤ mein kaun kaun sa Container 📦 Attach 🔗 hai

```bash
# Example --> docker network inspect my-custom-network

docker network inspect network_name
```
<br/>

- 👇 👇 Yah Command Sa Container 📦 ko inspect 👀 Kar sakte hain

```bash
# Example Name -->  docker inspcet funny_fermat
# Example id -->  docker inspcet 5abc9ee2ed05

docker inspect container_name Ya Fir container_id

```
