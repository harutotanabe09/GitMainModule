#### 　サブモジュールの作り方

メインモジュールを作成する

メインモジュールの中に以下のコマンドを叩くとサブモジュールとして連携できる

例）メインモジュールにBootstarpのモジュールを入れる

```shell
git submodule add https://github.com/twbs/bootstrap.git bootstrap
git add bootstrap
git commit -m "Add Twitter Bootstrap as a submodule"
```

↓　プッシュすると以下のようにコミットIDが付与された形で管理できる

 別々のリポジトリで管理する形になる。

![image-20190928092555748](./image-20190928092555748.png)

※　Dockerを管理するとき、
　  アプリケーションのソースコードとインフラの構築コードで分離することができるので便利

#### サブモジュールの更新

```shell
git submodule update
```