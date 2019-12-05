# Soseki-LSTM
2017年に経済学部のゼミ（データサイエンス）で個人的に取り組んだ「漱石っぽい文章を作ろうプロジェクト」の記録

## 手順
1. 夏目漱石の作品を青空文庫からダウンロード
2. 全てをひらがなに加工
3. LSTM または Bidirectional LSTM による学習
4. 文章生成

## データ `./data`
文字コードはUTF-8  
- `./data/soseki_raw`  
    青空文庫からダウンロード  
    https://www.aozora.gr.jp/index_pages/person148.html  
    おそらく全作品（要確認）  
    旧字によるタイトルの被りをなくしている。
- `./data/soseki_processed`  
    加工済みデータ  
    - `soseki_all.txt`  
        全作品を一つのファイルに繋げただけのもの
    - `soseki_all_hiragana.txt`
        全作品をひらがなに加工したもの
        
## 結果例 `./result`
LSTMとBidirectional LSTMの結果例を載せている。  
ほとんど意味を成していないがなんとなく昔の言葉遣いっぽい特徴は現れている。  
文章生成に使ったスクリプトは載せていないが、以下を参考にした。
https://github.com/fchollet/keras/blob/master/examples/lstm_text_generation.py
