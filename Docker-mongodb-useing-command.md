# Docker MongoDB RUN Commands

### [Docker mongo image link check now](https://hub.docker.com/_/mongo)

<br/>
<br/>
<br/>

- 👇 Yah Command MongoDB image ko pull karne ka hai

```bash
docker pull mongo
```

<br/>

- 👇 Is Tarike se mangoDB ki image ko RUN kar sakte hai

```bash
docker run -d --name mymongo -p 27020:27017 -e MONGO_INITDB_ROOT_USERNAME=mongoadmin -e MONGO_INITDB_ROOT_PASSWORD=scecret mongo
```

<br/>

- 👇 Yah Command Se Docker Volume Attach Karne ke sath hi mongo DB ko RUN kar sakte hain

```sh
docker run -d -p 27020:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password --name mongodbDatabase -v customvolumecreate:/data/db mongo
```

<br/>

- 👇 Is Url Se Connect kar sakte hain MongoDB ko MongoDB Compass se

```bash
mongodb://mongoadmin:scecret@localhost:27020/
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Same network mongoDB and nodejsAppImage connect kar sakte hain

<br/>

- 👇 Yah command Se Khud ka custom network create kar sakte hain

```bash
docker network create -d bridge my-custom-network
```

<br/>

- 👇 Yah command se Check & Dhkh 👀 kar sakte hain kaun kaun sa network available hai

```bash
docker network ls 
```

<br/>

- 👇 Is Tarike se mongo DB image ka customer network ke sath RUN 🏃‍♀️ kar sakte hain

```bash
docker run -d -p 27020:27017 --net my-custom-network -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=password --name mongodockerwala mongo

```

<br/>

- 👇👇 Is Tarike nodejs server ko customer network ke sath RUN 🏃‍♀️ kar sakte 

```bash
# Example --> docker run -d -p 4444:4444 -e PORT=4444 -e MONGO_URL=mongodb://admin:password@mongodockerwala --net my-custom-network somadev-server

docker run -d -p 4444:4444 -e PORT=4444 -e MONGO_URL=mongodb://admin:password@container_name --net my-custom-network somadev-server
```

<br/>

- 👇

```bash

```

<br/>

- 👇

```bash

```

<br/>

- 👇

```bash

```

<br/>

- 👇

```bash

```

<br/>

- 👇

```bash

```

<br/>
