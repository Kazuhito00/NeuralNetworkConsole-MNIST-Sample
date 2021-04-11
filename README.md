# NeuralNetworkConsole-MNIST-Sample
[Neural Network Console](https://dl.sony.com/ja/)でMNISTを学習するサンプルです。<br>
<img src="https://user-images.githubusercontent.com/37477845/114303458-30c28f00-9b09-11eb-80ad-a7170a623c67.png" width="60%"><br><br>
本リポジトリには以下の内容を含んでいます。<br>
* Jupyter Notebook：データセットダウンロード、保存
* Neural Network Console：学習、構造自動探索
* Neural Network Console：ONNXファイルエクスポート
* Jupyter Notebook：推論


# Requrement(Neural Network Console)
* Neural Network Console 2.0

# Requrement(Python)
* numpy 1.18.5 or later
* pandas 1.1.4 or Later
* onnxruntime 1.5.2 or later 

# Directory
<pre>
│  01_create_dataset.ipynb
│  05_inference_sample.ipynb
│
├─01.original_data
│      
├─02.data
│      
├─03-01.nnc_train_data
│      
├─03-02.nnc_test_data
│      
├─04.nnc_project
│  │  mnist.sdcproj
│  │  
│  └─mnist.files
│              
└─05.model

</pre>
<details open>
<summary>ディレクトリ内容</summary>

### 01_create_dataset.py
データセット作成用のスクリプトです。<br>
01.original_dataのデータをNeural Network Consoleに読み込める形にします。

### 04_inference.ipynb
モデル推論用のスクリプトです。<br>
Neural Network ConsoleからエクスポートしたONNXファイルを用いて推論を行い、submission.csvを作成します。

### 01.original_data
Kaggle Titanicの[データセット](https://www.kaggle.com/c/titanic/data)です。

### 02.data
01_create_dataset.pyを用いて前処理を行いNeural Network Consoleで読み込める形にしたデータセットです。

### 03-01.nnc_train_data

### 03-02.nnc_test_data

### 04.nnc_project
Neural Network Consoleのプロジェクトファイルです。

### 05.model
学習後にエクスポートしたONNXファイルです。

</details>

# Model
モデル構造は以下の通りです。<br>
* 自動探索開始時<br><img src="https://user-images.githubusercontent.com/37477845/114264511-5cb91400-9a26-11eb-97ae-99a983481698.png" width="40%">
* 自動探索実施後に性能が良かったもの<br><img src="https://user-images.githubusercontent.com/37477845/114264502-4ca13480-9a26-11eb-86f9-a1f3080ee28f.png" width="40%">

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)

# License 
Single-Hand-Localization is under [Apache v2 License](LICENSE).

