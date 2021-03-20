# ①Preprossesing
## ライブラリのインポート 
## データの読み込み、シャッフル、学習データと評価データの分割 
## データセットの作成 
### データセットクラスの定義
データファイル、transfromを引数とした__init__関数  
データファイルの長さを返す__len__関数  
指定インデックスのデータを読み込み、transformを通す__getitem__関数  
### パラメータの定義 
model,device,target_num,ir,batch_size,num_workers,epochs 
### transformの設定及びデータセットクラスへの適用
### データローダの定義　
# ②Learning 
## モデルの定義 
## モデルのインスタンス作成
## 最適化関数定義 
## loss関数定義 
## 学習モデル関数の定義し学習 
model,criterion,optimizer,num_epochs,is_saved(モデルを保存するかどうか）を引数とする。 
# ③Predicting 
## 推論用データセットの作成 
### transformの設定 
### テストデータセットクラスの定義 
### データセットのインスタンス作成 
### データローダの作成 
## 未知のデータに対する推論 
### モデルの定義 
### モデルのインスタンス作成 
学習したモデルをロード 
### 最適化関数定義 
### loss関数定義 
## 提出ファイルの作成 
### sample_submit.csvの読み込み 
### データローダからデータを取得し予測 
予測結果はsample_submitデータに書き込み保存
