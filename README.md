# Document Analysis
情報システム分析論のDocument Analysisの課題の提出フォルダ

## Assignment1(Document Clustering)
- 正規表現
- Clustering
- tf-idf
- K-means
- Principal Component Analysis (PCA)

./Data内にある文書(301個)をクラスタリング。
正規表現や置換により記号や数字の前処理を行った後、tf-idfでベクトル化。その後、K-meansで文書をクラスタリング。
K-meansは以下の2通りで計算している。

- scikit-learn (距離:Euclid Distance)
- nltk (距離:Cosine Distance)

分析として主成分分析による可視化やKの値を変更した時の比較も行なっている。(scikit-learnでのK-meansを使用)

### Assignment_1.ipynb
jupyter-notebookによる実行ファイル
### assignment_1_tf-idf.csv
各文書のtf-idfの値の一覧

## Assignment2(Topic Modeling)
- 正規表現
- LDA

./Data2内にある文書(1001個)をトピック分析。
正規表現や置換により記号や数字の前処理を行った後、
LDAを用いてトピック分析をし、
その後に可視化を行った。

分析としてトピック数を変えた時の結果の比較も行なっている。

### Assignment_2.ipynb
jupyter-notebookによる実行ファイル


## Data
データ(1000個)は以下のサイトから取得:

https://www.kaggle.com/datasets/jensenbaxter/10dataset-text-document-classification?resource=download

Assignment1では、
Business, Entertainment, Food, Politics, Sport, Technologieから50個ずつ(1-50)文書を取得。
加えて、オリジナルのテキスト一つ(music)を追加し、計301個使用。

Assignment2では、
Business, Entertainment, Food, Graphics, Historical, Medical, Politics, Space, Sport, Technologieの各ジャンルから100個ずつ文書を取得。
加えて、オリジナルのテキスト一つ(music)を追加し、計1001個使用。

