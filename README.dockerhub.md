# ubuntu-rdp in iganari

## 概要

Ubuntu に Xfce をインストールし、 RDP 接続を可能したもので、[@Rosyuku](https://github.com/Rosyuku) の [GitHub | ubuntu-rdp](https://github.com/Rosyuku/ubuntu-rdp) (and [Docker Hub | ubuntu-rdp](https://hub.docker.com/r/rosyuku/ubuntu-rdp)) を Fork し、カスタマイズしたものです
 
多謝 (-人-)

## コンテナイメージを pull して起動する

+ [Docker Hub | iganarix/ubuntu-rdp](https://hub.docker.com/repository/docker/iganarix/ubuntu-rdp) からコンテナイメージを直接取得して起動する

```
docker run --rm -it -p 13389:3389 -p 10022:22 --shm-size=256m iganarix/ubuntu-rdp:latest
```

+ RDP ツール (例えば Microsoft Remote Desktop) を用いて `127.0.0.1:13389` にログインする

![](https://raw.githubusercontent.com/iganari/ubuntu-rdp/master/img/04.png)

![](https://raw.githubusercontent.com/iganari/ubuntu-rdp/master/img/05.png)

![](https://raw.githubusercontent.com/iganari/ubuntu-rdp/master/img/06.png)

## 自分好みにカスタマイズする

[Docker Hub | iganarix/ubuntu-rdp](https://hub.docker.com/repository/docker/iganarix/ubuntu-rdp) のイメージを Dockerfile の FROM に使ってカスタマイズする

+ Dockerfile

```
FROM iganarix/ubuntu-rdp:latest

~
~
```

## もっと自分好みにカスタマイズしたい場合

[GitHub | iganari/ubuntu-rdp](https://github.com/iganari/ubuntu-rdp#readme) を clone してカスタマイズする

## まとめ

Have fan! :)
