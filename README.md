Example Docker Build 
=========

Getting started
---------------

Go to [Play with Docker](https://www.play-with-docker.com). Add 2 New Instances. 

Run these commands in your first instance:
```
git clone https://github.com/dockerbelfast/build-example.git
cd build-example
ls
```

Step 1 Build:
```
docker build -t hello-belfast-image .
```
Step 2 Ship:
```
docker login -u belfast -p <password>
docker tag hello-belfast-image belfast/hello-belfast-image:<your own initials>
docker push belfast/hello-belfast-image:<your own initials>
```

Run in these commands in your first instance:

Step 3 Run:
```
docker container run my-hello-belfast belfast/hello-belfast-image:<your own initials> 
```
