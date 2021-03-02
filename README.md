## 概要

ギグワーククエストのオレンジチームのコード管理リポジトリ

## コードの管理方法

各自ブランチを切って、切ったブランチの中でコード管理を行う

## 注意点

- 他の人のブランチにプッシュ等はしない（切り替えてローカル環境で実行とかはOK）
- inputデータなど管理する必要のないファイルはpushしない

## 使い方流れ

下記のサイトを参考に最低限の使い方を下記に記載してます！

https://tracpath.com/bootcamp/learning_git_firststep.html

1. 本リポジトリをローカルにクローン（コピー）

本リポジトリを自身のローカル環境にcloneする事で本リポジトリで管理されているファイル&管理履歴がローカル環境にコピーされます。

cloneのコマンドは以下の２種類です。

```
git clon https://github.com/AI-QUEST-TEAM4/model_verification.git # HTTP認証
git clon git@github.com:AI-QUEST-TEAM4/model_verification.git # SSH認証
```

* 認証の方法が違うだけで結果は一緒です。
* 個人的には下のSSH認証の方が後が楽なのでおすすめですが鍵の設定（詳しくは下記のサイト参照）が必要になります。

https://qiita.com/shizuma/items/2b2f873a0034839e47ce

2. ブランチを切る

自分のコードを管理する用のブランチを切ります。

```
git checkout -b (ブランチ名) # 新規ブランチを作りそれをカレントブランチにします
```

3. ローカルで作業

4. 作業したファイルを追加

ローカルで作業したファイルをgitに追加します。

```
git add <filename>
git add *              # 変更があったファイルをすべて索引に追加します
```

5. 作業をコミット
続いて作業内容をコミットします。

```
git commit -m "初めてのコミット"
```

6. リモートリポジトリにプッシュ
ローカルリポジトリに反映した内容をリモートリポジトリ（githubで管理してるリポジトリ）にプッシュ（同期）します。

branchnameは自分で切ったブランチ名になります。

初回のプッシュでリモートリポジトリに自分のブランチが作成されます。

```
git push origin (ブランチ名)
```

7. 上記の3〜6を繰り返して変更履歴をgitに記録

## 参考サイト

* gitの仕組みがわかりやすく載っていたので最初に読むのにおすすめです

https://tracpath.com/bootcamp/learning_git_firststep.html

* gitのコマンド忘れた時によく見てます

https://qiita.com/fukumone/items/73e1a9a62c5e4454263b
