# Docker
Step 1 : Build the container using this command 
``` 
docker build --tag mnist-hogwild .
```
Step 2 : Run this command to run the container 
```
docker run --rm -it mnist-hogwild
```
Step 3 : You can also specify the batch size using -
```
docker run --rm -it mnist-hogwild --batch-size=2
```

You can also see the images using the follwing command
```
docker image ls
```

```
REPOSITORY      TAG        IMAGE ID       CREATED          SIZE
mnist-hogwild   latest     a13d0bef0408   21 minutes ago   2.73GB
python          3.9-slim   5da6ce3c33c6   13 days ago      125MB
```
You can also inspect the container using the follwing command 
```
docker inspect a13d0bef0408
```

You can also see the cpu usage by opeaning the bash terminal and type 
```
htop
```