# cloudera directorの環境構築作業メモ
## cloudera directorのinstall
### macの場合
homebrew使ったinstallが下記リポジトリ使うとできる  
[chezou/homebrew-cloudera: Homebrew Formulas for cloudera tools](https://github.com/chezou/homebrew-cloudera)

```
$ brew tap chezou/cloudera
$ brew install cloudera-director-server
$ cloudera-director-server-start
```

### [wip] dockerの場合

## AWS EC2でインスタンス構築
- centos7で建てる

## coudera directorのguiから設定
1. http://localhost:7189 にアクセス
2. 「Add Environment」から新しい環境を構築
3. アクセスキーとシークレットキーの入力が求められるので、AWS上でユーザーを作成して入力[3]
4. ssh keyは建てたインスタンスグループのを設定

# 参考資料
[1] [Cloudera Directorを入れてクラウドにCDHクラスタを作ろう – Cloudera Japan Official Blog](https://blog.cloudera.co.jp/getting-started-cloudera-director-35405d421084)  
[2] [Cloudera Director のインストール方法
](https://qiita.com/shiumachi/items/90649830cb9b45726d99)  
[3] [AWSアクセスキー作成
](https://qiita.com/miwato/items/291c7a8c557908de5833)