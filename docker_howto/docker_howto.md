# Docker howto

## 1. Dockerとは

クラウドプラットフォームでは多数の実行環境にサービスを実行するソフトウエアモジュールを自在に配置、稼働します。そのためにソフトエアモジュールを自在に実行環境上で配置、稼働するための共通フォーマットがあると便利ですね。

そのような共通フォーマットが Docker コンテナであり、そのコンテナを操作するツールがDockerです。

Docker 自体は様々なプラットフォームで稼働するアプリケーションですが、Dockerを使って以下のことができます。

コンテナの作成
イメージの作成
コンテナ、イメージの起動

たとえば、pythonで稼働するサーバーを動かしたい場合、もちろんローカルマシン上aの通常のOS上でpython処理系を動かしてその上でサーバーを起動することも可能ですが、Dockerを使うと、

1. python処理系をコンテナにインストール
2. そのコンテナをローカルのコンテナ実行環境で実行
3. 実行中のプロセスにログイン
4. python で python コードを実行

と言う方法でも python の処理が可能です。

もしローカルのコンピュータで python プログラムを実行したいだけなら、これはただ手間がかかるだけですが、このようにコンテナ化することで、このコンテナはローカルのコンテナ実行環境だけでなく、あらゆるクラウド環境で無限といえる実行リソースに展開して実行することができます。

別のいいかたをすれば、コンテナというのはクラウド環境のための実行用ファイルの形態で、Dockerはその作成や管理を行うツールということもできます。

そしてコンテナは通常、クラウド環境上で多数の計算リソースに展開されて平行実行されます。したがってこれまでの、単一CPUのコンピュータの実行モジュールは、ロードと実行がほぼ一体であったのに対し、コンテナの実行には、

1. インスタンス 実行リソースの割りあ宛てp
2. デプロイ 実行モジュールへのコンテナの割り当て
3. 実行 プロセスの起動
 
という手順をとります。

# 2. Docker の準備
## 2.1 必要なもの

以下はあらかじめ用意します。

(1) Dokcer リポジトリのアカウント用のidとpasswd

id (email アドレス) とパスワードを用意しておきます
これはなんでもかまいません。忘れないように記録しておきます。

(2) GitHub のアカウント
これはあった方が便利ですがなくてもかまいません。

## 2.2 必要なソフトウエア

(1) Windows 11
Macintoshの方がポピュラーであるようですがこの資料ではWindwos 11 を使って説明をします。

(2) WSL
後でインストールします

(3) Docker Desktop
後でインストールします

(4) VSCode
あった方が便利なので後でインストールします

# 2 インストール

# 2.1 WSL2 のインストール

WSL　は Windows Subsystem for Linux といい、Windows を Linux として利用するための拡張モジュールです。Windows は Linux ベースではありませんが、Linux の機能を持っているので、WSL を追加することで、Linxu と同じように使うことがｄけいます。つまり Linux のアプリケーションプログラムやコマンドをすべて利用できるようになります。





![画像](image/test.png "サンプル")