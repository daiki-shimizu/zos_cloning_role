IBM z/OS Cloning role 
=========
IBM z/OS Cloning roleは、z/OSをクローニングするドライバーシステムで利用されるJCLを作成します。これにより、新システムを構築する作業の効率化を図ります。



特徴
========
以下のテンプレートを使ってJCLを作成し、ドライバーシステムに転送します。


1. 事前準備
- 新システムのDASDの初期化

2. カタログの作成
- 新システムのマスターカタログの作成
- 新システムのSSA(System Specific Alias)の作成

3. 既存設定の引継ぎ
- マスターシステムのマスターカタログのインポート
- マスターシステムのIODFのコピー
- マスターシステムの既存データセットのコピー
- マスターシステムのマスターカタログのエクスポート

4. システムデータセットの作成
- ページデータセットの作成
- JES2スプール関連データセットの作成
- SMF関連データセットの作成
- カップルデータセットの作成

5. IPL Textの作成

6. 後処理
- SSAの削除
- 新システムのマスターカタログのエクスポート 


前提
------------
IBM z/OS core collectionをAnsibleコントローラーノード側に導入しておく必要があります。


Copyright
=========
© Copyright IBM Corporation 2020

