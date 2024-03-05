***** Redis *****
Instructiunile de instalare a serviciului Redis le gasim pe site-ul
https://hub.docker.com/_/redis
1. Instalam Redis, in CMD lasam comanda
docker pull redis
2. Lansam Redis, in CMD lasam comanda
docker run --name redis-cache -p 6379:6379 -d redis

Pentru a vedea datele din redis avem nevoie de un Redis GUI
https://github.com/qishibo/AnotherRedisDesktopManager/releases
in GUI configuram accesul local la Redis
localhost@6379

***** Docker compose *****
Lansam CMD cd la mapa unde sunt fisierele de mai sus (cd C:\PROJECTS\Dana\PAD3\Service)
Lansam comenzile:
docker-compose build
docker-compose up

***** Docker hub *****
docker tag pad/service.api:linux-latest danieladoni01/service.api
docker login
docker push danieladoni01/service.api

***** Install *****
cd C:\PROJECTS\Dana\PAD3\Service\install
docker-compose build
docker-compose up

***** Service *****
Link-ul de lansare a serviciului dupa instalare
http://localhost:7101/swagger/index.html

***** Postman Collection *****
https://github.com/DoniDaniela/PAD3/blob/main/PAD3.postman_collection.json
