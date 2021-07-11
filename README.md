# ubuntu-rdp in iganari

## 概要

Ubuntu に Xfce をインストールし、 RDP 接続を可能したもので、[@Rosyuku](https://github.com/Rosyuku) の [GitHub | Rosyuku/ubuntu-rdp](https://github.com/Rosyuku/ubuntu-rdp) (and [Docker Hub | rosyuku/ubuntu-rdp](https://hub.docker.com/r/rosyuku/ubuntu-rdp)) を Fork し、カスタマイズしたものです
 
多謝 (-人-)

## Dockerfile から起動する

+ Docker Compose で起動する

```
git clone https://github.com/iganari/ubuntu-rdp.git
cd ubuntu-rdp
```
```
docker-compose up --build
```

+ RDP ツール (例えば Microsoft Remote Desktop) を用いて `127.0.0.1:33890` にログインする

![](./img/01.png)

![](./img/02.png)

![](./img/03.png)

## コンテナイメージを pull して起動する

+ [Docker Hub | iganarix/ubuntu-rdp](https://hub.docker.com/repository/docker/iganarix/ubuntu-rdp) からコンテナイメージを直接取得して起動する

```
docker run --rm -it -p 13389:3389 -p 10022:22 --shm-size=256m iganarix/ubuntu-rdp:latest
```

+ RDP ツール (例えば Microsoft Remote Desktop) を用いて `127.0.0.1:13389` にログインする

![](./img/04.png)

## 自分好みにカスタマイズする

+ 推奨 ---> [自分でイメージから作成する](./README.md#自分で-dockerfile-から作成する)
+ お手軽にやりたい人 ---> [Docker hub のイメージをカスタマイズする](./README.md#docker-hub-のイメージをカスタマイズする)

### 自分で Dockerfile から作成する

この Repository を Fork するか、本家の Respotiroy を Fork してカスタマイズする

それをプライベートのレジストリに登録し使用する

### Docker hub のイメージをカスタマイズする

[Docker Hub | iganarix/ubuntu-rdp](https://hub.docker.com/repository/docker/iganarix/ubuntu-rdp) のイメージを Dockerfile の FROM に使ってカスタマイズする

+ Dockerfile

```
FROM iganarix/ubuntu-rdp:latest

~
~
```