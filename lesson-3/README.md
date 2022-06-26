# build docker image

docker build -t glls/building-apps . 

# build multi platform docker image

docker buildx build -t glls/building-apps:0.1  --push --platform=linux/arm64,linux/amd64 .

docker manifest inspect glls/building-apps:0.1

