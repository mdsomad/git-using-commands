# Doker Using Commands

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Docker Install

- 👇 Windows Docker Download Link
- [Docker Download Website Link](https://www.docker.com/products/docker-desktop/)
  <br/>
  <br/>
  <br/>
  <br/>
  <br/>
  <br/>

- 👇 Yah command se check kar sakte hain docker install hai kya Nahin Aur Docker Ka Version

```sh
docker -v
```

<br/>

- 👇 Yah command se docker ka service start kar sakte hain

```sh
systemctl start docker.service
```

<br/>

- 👇 Yah command se docker ka service status check kar sakte hain

```sh
systemctl status docker.service
```

<br
  
- 👇 Pre Defined

```sh
DOCKER IMAGES

docker pull nginx

docker run -p 8080:80
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

- 👇 Yah command se doctor Mein local machine Mein login 👤🔐🔑 kar sakte hain

```sh
docker login
```

<br/>

- 👇 Yah command se bhi doctor ka All images 🖼️ dekh h 👀 sakte hain

```sh
docker images
```

<br/>

- 👇 Yah donon command se docker image 🖼️ ko Create and Docker Hub Mein push and upload 📤 kar sakte hain

```sh
docker build -t mdsomad/mywebapp-demo:01 .
docker push mdsomad/mywebapp-demo:tagname
```

