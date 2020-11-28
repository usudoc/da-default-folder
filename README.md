・configs  # 諸設定が記載されたjsonファイルを保存
  - default.json  # 「利用している特徴量」「学習器のパラメータ」など
・data
  - input  # 入力データ
    - external  # kaggle等に挙げられたサードパーティー製のデータ
    - interim  # データ処理を行った中間データ
    - processed  # 予測等に最終的に使用するデータ
    - raw  # コンペティションで与えられた生データ
  - output  # 出力データ
    - raw  # コンペティションで与えられた生データ
・models  # 推論後のモデルを保存する場所
・notebooks  # EDAなど
・src  # スクリプト群
  - data  # データをダウンロードしたり生成したりするスクリプト
  - features  # 生データをモデリング用に変換するスクリプト
  - models  # モデルによる訓練と予測を行うスクリプト
    # 入力:pandas.DataFrame、パラメータ
    # 出力:予測結果
    - predict_model.py
    - train_model.py
・README.rd