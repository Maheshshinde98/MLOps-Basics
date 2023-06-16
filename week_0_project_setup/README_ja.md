**Note: ライブラリを探索し、その使い方を学ぶことが目的です。SOTA モデルを作るためではありません**。

## Requirements

このプロジェクトは Python3.8 を使用しています

以下のコマンドで仮想 env を作成します：

```bash
conda create --name project-setup python=3.8
conda activate project-setup
```

必要なものをインストールします：

```bash
pip install -r requirements.txt
```

## Running

### Training

要件をインストールした後、モデルをトレーニングするために、単純に実行します：

```bash
python train.py
```

### Inference

トレーニング後、コード内のモデルチェックポイントパスを更新して実行する

```bash
python inference.py
```

### Running notebooks

ノートブックの実行に[Jupyter lab](https://jupyter.org/install)を使用しています。

virtualenv を使っているので、`jupyter lab`というコマンドを実行すると、virtualenv が使われる場合と使われない場合があります。

virutalenv を確実に使用するためには、`jupyter lab`を実行する前に以下のコマンドを実行してください。

```bash
conda install ipykernel
python -m ipykernel install --user --name project-setup
pip install ipywidgets
```