# ubuntu-rdp in iganari

## 概要

改造版

+ Fork 元
  + [GitHub](https://github.com/Rosyuku/ubuntu-rdp)
  + [Docker Hub](https://hub.docker.com/r/rosyuku/ubuntu-rdp)

## ローカルで実行起動する

+ Docker Compose で起動する

```
docker build . --tag hogehoge
docker run --rm -it -p 13389:3389 -p 10022:22 --shm-size=256m hogehoge
```


```
docker-compose up --build
```

```
127.0.0.1:33890
```

![](./img/01.png)

![](./img/02.png)

![](./img/03.png)

## Docker Hub に登録している版を起動する

WIP

## 自分好みにカスタマイズする

### [お手軽] Docker hub のイメージをカスタマイズする

WIP

### [推奨] 自分でイメージから作成する

この repo を fork するか、大本を fork してカスタマイズしていく

