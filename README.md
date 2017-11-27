## docker-compose for wordpress
--------------------

1. install Docker
2. creating container for storing data  $ `docker build -t dataonly .`
3. check images  $ `docker images dataonly`
4. run  $ `docker run -d --name dataonly dataonly`
5.  $ `docker-compose up -d`
6. open http://localhost:80

```
<command >
 $ docker-compose ps
 $ docker-compose stop 
 $ docker-compose rm
```

* Making backup  $ `docker export dataonly > backup.tar`
* Restore data   $ `tar xvf backup.tar`
