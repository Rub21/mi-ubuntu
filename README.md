# mi-ubuntu

It's a straightforward container that comes with all the necessary programs installed for managing an EKS cluster. This setup allows me to quickly launch a container and get to work, especially if I need to conduct user permission tests on the cluster.

## Build
```sh
docker login
docker push rub21/miubuntu:v1
```

## Run
```sh
docker run -it \
    -v $(pwd):/mtn \
    --rm \
    rub21/miubuntu:v1 bash
```