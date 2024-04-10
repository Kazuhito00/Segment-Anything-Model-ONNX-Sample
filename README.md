# Segment-Anything-Model-ONNX-Sample
[facebookresearch/segment-anything](https://github.com/facebookresearch/segment-anything) のエンコーダー/デコーダーをONNXに変換し、推論するサンプルです。<br>
推論スクリプトは、前処理、後処理を含めPyTorch依存の処理は使用しない方針です。

https://github.com/Kazuhito00/Segment-Anything-Model-ONNX-Sample/assets/37477845/18428108-49ef-4683-80c8-4ea2a4fce62c

# Usage
#### ONNX変換、推論テスト
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kazuhito00/Segment-Anything-Model-ONNX-Sample/blob/main/Segment-Anything-Model-ONNX.ipynb)<br>
Colaboratoryでノートブックを開き、上から順に実行してください。<br>

#### 簡易デモ
Colaboratoryノートブックで変換したONNXファイルを「onnx_model」ディレクトリに格納し、
以下コマンドでデモを起動してください。<br>
```
python demo.py
```
* --image<br>
画像ファイルの指定<br>
デフォルト：sample.png
* --encoder<br>
エンコーダーONNXファイルのパス<br>
デフォルト：onnx_model/vit_b_encoder.onnx
* --decoder<br>
デコーダーONNXファイルのパス<br>
デフォルト：onnx_model/vit_b_decoder.onnx

# Note
サンプルの画像は[ぱくたそ](https://www.pakutaso.com/)様の「[トゲトゲのサボテンとハリネズミ](https://www.pakutaso.com/20190257050post-19488.html)」を使用しています。

# License 
Segment-Anything-Model-ONNX-Sample is under [Apache-2.0 license](LICENSE).

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)
