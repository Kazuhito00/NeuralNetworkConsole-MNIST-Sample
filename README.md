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
MNISTデータセットをダウンロードし、02.dataに格納します。

### 05_inference_sample.ipynb
モデル推論用のスクリプトです。<br>
Neural Network ConsoleからエクスポートしたONNXファイルを用いて推論を行うサンプルです。

### 01.original_data
01_create_dataset.py実行時に、MNISTデータセット(解凍前)を格納するディレクトリです。

### 02.data
01_create_dataset.py実行時に、回答したデータセットを格納するディレクトリです。

### 03-01.nnc_train_data
Neural Network Console用の学習データを格納するディレクトリです。<br>
Neural Network Consoleで「データセットを作成」し、出力ディレクトリに指定してください。<br>
<img src="https://user-images.githubusercontent.com/37477845/114304248-2b674380-9b0d-11eb-9071-e3a96385c0be.png" width="70%">

### 03-02.nnc_test_data
Neural Network Console用の検証データを格納するディレクトリです。<br>
Neural Network Consoleで「データセットを作成」し、出力ディレクトリに指定してください。<br>
<img src="https://user-images.githubusercontent.com/37477845/114304313-6d908500-9b0d-11eb-8f3b-d7b1d0c3248e.png" width="70%">

### 04.nnc_project
Neural Network Consoleのプロジェクトファイルです。

### 05.model
学習後にエクスポートしたONNXファイルです。

</details>

# Model
モデル構造は以下の通りです。<br>
* 自動探索開始時<br><img src="https://user-images.githubusercontent.com/37477845/114304517-8d747880-9b0e-11eb-8821-cfa8778647bb.png" width="70%">
* 自動探索実施後に性能が良かったもの<br><img src="https://user-images.githubusercontent.com/37477845/114304430-06270500-9b0e-11eb-92b5-4af0aac8f2a5.png" width="70%">
* 自動探索実施後に性能が良かったもの<br><img src="https://user-images.githubusercontent.com/37477845/114304451-29ea4b00-9b0e-11eb-8c7a-51518df62804.png" width="70%">


# Author
高橋かずひと(https://twitter.com/KzhtTkhs)

# License 
Single-Hand-Localization is under [Apache v2 License](LICENSE).

