# ubuntu-rdp in iganari

## 概要

Ubuntu に Xfce をインストールし、 RDP 接続を可能したもので、[@Rosyuku](https://github.com/Rosyuku) の [GitHub | ubuntu-rdp](https://github.com/Rosyuku/ubuntu-rdp) (and [Docker Hub | ubuntu-rdp](https://hub.docker.com/r/rosyuku/ubuntu-rdp)) を Fork し、カスタマイズしたものです
 
多謝 (-人-)

## ローカルで実行起動する

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

## Docker Hub に登録している版を起動する

WIP

## 自分好みにカスタマイズする

+ 推奨 ---> [自分でイメージから作成する]
+ お手軽にやりたい人 ---> [Docker hub のイメージをカスタマイズする]


### 自分でイメージから作成する

この Repository を Fork するか、本家の Respotiroy を Fork してカスタマイズする

それをプライベートのレジストリに登録し使用する

### Docker hub のイメージをカスタマイズする

WIP



