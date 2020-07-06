#### Dockerizing a React app

Login to Docker Hub

```zsh
$ docker login
```

create a React container

```zsh
$ docker build -t {yourDockerUsername}/react-app:1.0.0 .
```

Test the React container by running it. It should be visible at localhost:8080

```zsh
$ docker run -p 8080:80 {yourDockerUsername}/react-app:1.0.0
```

Push the container to your Docker Hub account repository

```zsh
$ docker push {yourDockerUsername}/react-app:1.0.0
```
