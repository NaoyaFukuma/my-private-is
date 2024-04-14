# private-isu-playground

### CI/CD環境の構築練習

プッシュ時の自動レビューを追加

##### terraformでの環境構築
 - [ ] terraformを使って、クラウド上にappとbenchを構築
   - [ ] ローカル環境からインターネット越しにAPPインスタンスとBENCHインスタンスにアクセスする。
   - [ ] VPCは、一つのパブリックサブネットを有する。
   - [ ] 各インスタンスは、private-isuのリポジトリREADME記載のAMIを利用する。

|種類|AMI ID|AMI NAME|推奨インスタンスタイプ|
|---|---|---|---|
|APP|ami-0937f4bab7bea4382|catatsuy_private_isu_amd64_20240323|c7a.large|
|BENCH|ami-015450874c83c16e5|catatsuy_private_isu_bench_amd64_20240323|c7a.xlarge|

   - [ ] AMIの情報をソース情報として取得する。
   - [ ] これらの環境をterraformで定義する。

##### github actions  
 - [ ] github actionsを使って、プッシュ時にクラウド上にデプロイして、ベンチマークを実行
 - [ ] トリガーをディレクトリごとに分けて、必要なものだけをデプロイし直すように設定
 - [ ] ベンチマークの実行時に、クエリの解析やローテートも、github actionsで行う

#### 実験
   - [ ] DBのマイグレーションツールの導入
   - [ ] 解析ツールの導入
   - [ ] DBの修正
   - [ ] appコードの修正
   - [ ] nginx設定の修正

