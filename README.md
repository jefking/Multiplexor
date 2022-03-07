# Multiplexor

## BUILD
```
cd ingress
sudo docker build . -t mvp/ingress
```

```
cd listen
sudo docker build . -t mvp/listen
```

## RUN
Listen 1
```
docker run -it -p 9090:80 mvp/listen
```
Listen 2
```
docker run -it -p 9091:80 mvp/listen
```
Ingress
```
docker run -it -p 9080:80 mvp/ingress
```