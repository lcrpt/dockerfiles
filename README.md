# dockerfiles

## redis
```sh
$ docker build -t redis redis/;
$ docker run -d -p 6379:6379 redis;
```

## adonisjs
```sh
$ docker build -t adonis:1.0.0 adonisjs;
$ docker save -o adonis.tar adonis:1.0.0;
$ docker load -i adonis.tar;
$ docker run --name=adonis -p 12345:80 -v $PWD/src:/var/www adonis:1.0.0;
```
