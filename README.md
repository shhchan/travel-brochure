# 旅行のしおり用リポジトリ
<img src="http://img.shields.io/badge/-LaTeX-008080.svg?logo=latex&style=flat">
これは旅行のしおり用のリポジトリです。

# 始め方

## 作業場所にリポジトリを作成する

```shell
cd /path/to/your/working/directory
```
```shell
git init
```

## 旅行のしおり用リポジトリのソースをローカルにクローンする

```shell
git clone https://github.com/shhchan/travel-brochure.git
```

# 作業方法

## 最新の情報を取り込む

```shell
git pull
```

## ブランチを移動する
 ```shell
 git checkout ブランチ名
 ```

 ## ブランチをきる
 ```shell
 git branch -b 新しいブランチ名 origin/もってくるブランチ名
 ```

 ## ステージする
 #### 作業ツリーすべてステージ
 ```shell
git add -A
 ```
  #### 変更だけステージ
 ```shell
git add -u
 ```

 ## コミットする
 ```shell
 git commit -m "メッセージ"
 ```

 ## プッシュする
 ```shell
 git push origin プッシュ先のブランチ名
 ```
 ### 現在のブランチ名を指定せずにプッシュする
 ```shell
 git push -u origin HEAD
 ```

 # 取り消ししたいとき
  ## ステージから取り除く
  ```shell
  git reset HEAD
  ```

  ## 直前のコミットを取り消し
  ```shell
  git reset --soft HEAD^
  ```