# milkboy_cornflakes

忘れっぽいオカンが呟いてた特徴を入力すると，それがコーンフレークかどうかツッコミを入れてくれる分類器を作って遊んでみました．


## 実行例
```
$ python3 milkboy_main.py
(setting up...)
オカンが言うにはな、>>>牛乳とは合わないらしいねん
ほなコーンフレークちゃうかぁ...
オカンが言うにはな、>>>死ぬまで食べ続けれるらしいねん
ほなコーンフレークちゃうかぁ...
オカンが言うにはな、>>>朝に食べるのにちょうどいいらしいねん
それ、コーンフレークや！
オカンが言うにはな、>>>ご飯でもパンでもないらしいねん
ほなコーンフレークちゃうかぁ...
オカンが言うにはな、>>>ご飯の中の英雄らしいねん
それ、コーンフレークや！
もうええわ
```


## ディレクトリ構造
- milkboy_cornflakes/
  - entity_vector/
    - entity_vector.model.bin : [学習済みword2vecモデル](https://github.com/singletongue/WikiEntVec)
  - milkboy_data.csv ： データセット（100件）
  - milkboy_data.py ： データセット作成
  - milkboy_train.py ： 分類器モデル学習
  - milkboy_model.pickle ： 学習済み分類器モデル
  - milkboy_main.py : メインスクリプト
