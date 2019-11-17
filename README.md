# polisDeployment


### Build images and run

Clone required repos:


```
git clone https://github.com/g0v-it/polisMath.git
git clone https://github.com/g0v-it/polisServer.git
git clone https://github.com/g0v-it/polisClientParticipation.git
git clone https://github.com/g0v-it/polisClientAdmin.git
```

Build images:


```
docker build -t copernicani/polis_math -f polisMath/Dockerfile polisMath
docker build -t copernicani/polis_server -f polisServer/Dockerfile polisServer
docker build -t copernicani/polis_db -f polisServer/Dockerfile-db polisServer
docker build -t copernicani/polis_clientparticipation -f polisClientParticipation/Dockerfile polisClientParticipation
docker build -t copernicani/polis_clientadmin -f polisClientAdmin/Dockerfile polisClientAdmin
```

run stack:

```
docker-compose up -d
```



