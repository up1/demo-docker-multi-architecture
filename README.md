## Step to run
```
docker buildx create --name mybuilder --use --bootstrap
docker buildx build --platform linux/amd64,linux/arm64,darwin/arm64 -t demo:1.0 .

docker buildx build --push --platform linux/amd64,linux/arm64 -t somkiat/demo:1.0 .
```


**Reference**
https://www.somkiat.cc/docker-tips-multi-architecture-image/