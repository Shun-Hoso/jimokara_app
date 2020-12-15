# README

## 目次

- [概要](##概要)
- [実装機能](##実装機能)
- [使用パッケージ](##使用パッケージ)
- [開発](##開発)
- [その他](##その他)

## 概要
こちらはカラオケ好きのユーザーに特化した無料マッチングアプリケーションです。  
地域・年齢・性別を絞って集まりたいメンバーでイベントに参加ができます。  
会員の方はイベントの企画が自由にでき、非会員の方はイベントの参加のみ可能です。  
以下のリンク先から本アプリケーションへアクセスができます。

[本アプリケーション](http://########.jp)  

**以下のテストユーザーを使用してログインすることも可能です。**

#### テストユーザー
- Name: testuser1
- Email: jimokara.test@gmail.com


## 実装機能
- deviseを使用したユーザー管理機能（ユーザー登録・ユーザー削除・ログイン・ログアウト）
- OneSignalを使用したプッシュ通知機能
- Ransackを使用したイベント検索機能
- ActionCableを使用した非同期コメント機能
- Ajaxを使用した良いね機能
- RSpec単体テスト（モデル・コントローラー）
- RSpec結合テスト（Capybara使用）


## 使用パッケージ
- Rails
- MySQL
- Node.js
- AWS
- Docker


## 開発
こちらのガイドに従って、環境などを設定してください。
### データベース
本アプリケーションは、MySQLデータベースを想定しております。  
もしMySQLを使用されていない場合は、個別にインストールする必要がございます。  
<details><summary>MySQLの導入が済んでいない場合は行頭のタブを開き、その中のコマンド参考に準備をお願いします。</summary>

- MySQLをインストール（以下はMySQLバージョンを5.7に指定した例）

```
% brew install mysql@5.7
```

- MySQLのコマンドをどこからでも実行できるように使用シェルにパスを読み込む  
（以下はzshのシェルを使用した場合）

```
% echo 'export PATH="/usr/local/opt/mysql@5.7/bin:$PATH"' >> ~/.zshrc
% source ~/.zshrc
```

- MySQLの起動

```
% mysql.server start
```
</details>


### アプリケーションのインストールと起動

- リポジトリーをクローンします。

```
% git clone https://github.com/Shun-Hoso/jimokara_app.git
```

- リポジトリに移動します。

```
% cd jimokara_app
```

- Gemをインストールします。

```
% bundle install
```

- yarnをインストールします。

``` 
% yarn isntall
```

- データベースを作成します。

```
% rails db:create
```

- テーブルを作成します。

```
% rails db:migrate
```

- アプリケーションを起動

```
% rails s
```


## その他

### ポートフォリオサイト
[こちらは自身のポートフォリオサイトになります。](http://xxxxx.jp)

### 個人ブログ
[こちらは自身で書いたQiitaの記事一覧です。](http://xxxxx.jp
)

