# Soseki_LSTM
2017年の学部のゼミでやった「漱石っぽい文章を作ろうプロジェクト」の記録

## 手順
1. 夏目漱石の作品を青空文庫からダウンロード
2. 全てをひらがなに加工
3. LSTM または Bidirectional LSTM による学習
4. 文章生成

## 結果例 `./result`
LSTMとBidirectional LSTMの結果例を載せている。  
ほとんど意味をなしていないがなんとなく昔の言葉遣いっぽい特徴は現れている。  
文章生成に使ったスクリプトは載せていないが、以下を参考にした。
https://github.com/fchollet/keras/blob/master/examples/lstm_text_generation.py

## データ `./data`
文字コードはUTF-8
- `./data/soseki_raw`  
    青空文庫からダウンロード  
    おそらく全作品
- `./data/soseki_processed`  
    加工済みデータ  
    - `soseki_all.txt`  
        全作品を一つのファイルに繋げただけのもの
    - `soseki_all_hiragana.txt`
        全作品をひらがなに加工したもの
        
 
