# 機械学習について

## 目次
- 機械学習とは
- 機械学習を行う手順
  - データの読込みとデータの可視化
    - 基礎統計量の確認
    - データ集計
    - グラフ化
    - 相関関係
  - データの前処理
    - 欠損地の処理
    - データのスケール
    - カテゴリカル変数のエンコーディング
    - 他のテーブルとの結合
  - モデルの学習
    - 回帰分析
    - ロジステック回帰
    - 決定木
    - ランダムフォレスト
  - モデルの評価
    - [機械学習で使われる評価関数まとめ](https://qiita.com/monda00/items/a2ee8e0da51953c24da8)
- 実装例
- 事例
  - [チャットボット](https://www.topgate.co.jp/blog/google-service/13077)
  - [Posen](https://hi.posen.ai/)
  - [音声でカルテ自動生成](https://site.medimo.ai/)
- 機械学習の活用事例
  - 店舗の来客分析（データ分析）
  - 農家の生産量予測（データ予測）
  - アパレルの需要予測（データ予測）
  - チャットボットによる問い合わせ対応（自然言語処理） 
```text
## 機械学習の活用事例
1.店舗の来客分析（データ分析）
コンビニやスーパーをはじめとして、店舗の来客分析には機械学習が活用されています。

顧客導線をもとに店内のレイアウトを検討したり、年齢・性別・購入商品など多角的なデータを分析することで、より生産性の高い店舗運営を実現することが可能になります。

従来は店舗担当者の経験や勘に依存することが多かった商品陳列も、膨大なデータをもとに効率化を図ることができます。

2.農家の生産量予測（データ予測）
一次産業である農家でも機械学習が活用されています。気象データをもとに収穫量や収穫時期を予測することで、農作物の生産過程における無駄を排除します。

また、収穫作業に必要な作業員の人数も目処を立てることができるため、雇用の観点からも生産性を高めることができ、農作物の価格や需要を予測することで、廃棄量の削減にも直結します。

3.アパレルの需要予測（データ予測）
アパレルは流行があっという間に変化する業界です。そのため、過剰在庫や廃棄が大きな問題となっていますが、機械学習を活用することで流通データなどをもとに流行を予測し、適切な店舗運営に繋げることができます。

さらに、人工知能（ AI ）を活用した商品発注も現実化しており、発注に費す時間を削ることで店員は接客に集中することができ、店舗全体の生産性が向上します。

4.チャットボットによる問い合わせ対応（自然言語処理）
最近では、問い合わせ対応をチャットボット化する企業が増えてきました。チャットボットの裏側も機械学習の自然言語処理の技術が活用されています。

顧客からの問い合わせ対応をチャットボットで自動化することで、カスタマーサポート部門の工数削減に直結します。また、問い合わせ対応の時間短縮や人件費の削減にも繋がるため、企業の生産性向上を実現することができます。
```


## 参考資料
- [自動車環境性能の改善](https://quest.signate.jp/quests/10001)
- [自動車の走行距離予測](https://signate.jp/competitions/121/data)
- [スポーツのチケット価格の最適化](https://quest.signate.jp/quests/10006)
- [AWS HealthLake](https://aws.amazon.com/jp/healthlake/?nc1=h_ls)
- [PV・UU・セッション数とは？](https://tsunaweb.book.mynavi.jp/tsunaweb/tsuna/detail/id=5176)
- [Python + BigQuery の始め方](https://tech.revcomm.co.jp/get-started-bigquery-with-python)
- [https://qiita.com/MRO/items/9fb8d8226fccb99f3886](https://qiita.com/MRO/items/9fb8d8226fccb99f3886)
- [GA4のBigQueryスキーマ](https://docs.google.com/spreadsheets/d/1JNmpTtHkmBn-61_nTPMm-O2uzSPBU7PhpKvRb7Ro5Y0/edit?gid=0#gid=0)
- [MySQLから移行してBigQueryを少し使ってみた](https://qiita.com/y-encore/items/71adf46a3473216ea7cd)
- [IT初学者がカラムナデータベースを勉強してみた](https://future-architect.github.io/articles/20210419b/)
- [BigQueryとは？代表的な機能やGA4との連携方法まで徹底解説！](https://anymanager.io/ja/blog/big-query)
- [Hugging Faceとは何か？](https://www.sbbit.jp/article/cont1/122042)
- [Hugging Faceとは？](https://miralab.co.jp/media/hugging-face/)
- [pyannote.audioで簡単話者分離](https://qiita.com/sayo0127/items/e22fdc229d2dfd879f75)
- [Pythonで始める音楽制作: pydubライブラリ入門](https://qiita.com/Tadataka_Takahashi/items/0f8238936d209c1fad2c)
- [FFmpegのインストールと使用方法 （Rocky Linux 9.2 ）](https://qiita.com/24Century/items/33f92bfc960d5126f916)