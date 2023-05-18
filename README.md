# Document Analysis
情報システム分析論のDocument Analysisの課題の提出フォルダ

## Assignment1(Document Clustering)
----
- Clustering
- tf-idf
- K-means
- Principal Component Analysis (PCA)

./Data内にある文書(301個)をクラスタリング。
正規表現や置換により記号や数字の前処理を行った後、tf-idfでベクトル化。その後、K-means法で文書をクラスタリング。
分析として主成分分析による可視化やKの値を変更した時の比較も行なっている。

### Assignment_1.ipynb
jupyter-notebookによる実行ファイル
### assignment_1_tf-idf.csv
各文書のtf-idfの値の一覧

## Data
---
一部のデータ(300個)は以下のサイトから取得:

https://www.kaggle.com/datasets/jensenbaxter/10dataset-text-document-classification?resource=download

Business, Entertainment, Food, Politics, Sport, Technologieから50個ずつ(1-50)文書を取得

加えて、オリジナルのテキスト一つ(music)を追加