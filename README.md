# jupyter_java

This docker image provides the [IJava Kernel](https://github.com/SpencerPark/IJava).

## Run

```
docker run -it -p 8888:8888 --name java java
```

If you want to keep your notebooks persitently on your host machine, simply map the
volume that's used internally by the container:

```
docker run -it -p 8888:8888 --name java -v /my/host/notebooks:/home/jovyan/notebooks  java
```
