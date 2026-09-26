# Data Science Advanced

弘前大学「データサイエンス応用」で使用する教材・演習用リポジトリです。

この授業では、Pythonによるデータ分析・統計モデリング・機械学習に加えて、VS Code、Miniforge、Git / GitHubを用いたデータ分析プロジェクトの管理方法を学びます。

## Course objectives

この授業では、以下の能力を身につけることを目標とします。

- VS CodeとMiniforgeを用いてPython実行環境を構築する
- Pythonを用いてデータを処理・分析する
- NumPy、pandas、Matplotlibを用いてデータ分析を行う
- 統計モデリングや機械学習をPythonで実行する
- Gitを用いてコードや分析結果の変更履歴を管理する
- GitHub上のリポジトリを利用してプロジェクトを管理する
- Jupyter NotebookとPythonスクリプトを目的に応じて使い分ける
- AIによるコーディング支援を適切に利用し、生成されたコードを確認・検証する

## Repository structure

```text
ds_advanced/
├── README.md
├── environment.yml
├── notebooks/     # Jupyter Notebook
├── scripts/       # 実行用Pythonコード
├── src/           # 再利用するPythonモジュール
├── data/          # 授業用データ
└── exercises/     # 演習課題
```

### notebooks

授業で使用するJupyter Notebookを置きます。

データの確認、試行錯誤、可視化、統計分析など、対話的な分析に使用します。

### scripts

単独で実行するPythonプログラム（`.py`）を置きます。

### src

複数のNotebookやPythonプログラムから再利用する関数やモジュールを置きます。

### data

授業で使用するデータを置きます。

公開可能で、再配布に問題のないデータのみを格納します。

### exercises

授業中および宿題で使用する演習課題を置きます。

## Python environment

この授業では、Miniforgeを利用してPython環境を管理します。

授業用の環境名は

```text
ds
```

とし、Python 3.12を使用します。

リポジトリに含まれる `environment.yml` から環境を作成できます。

```bash
conda env create -f environment.yml
```

作成した環境を有効にします。

```bash
conda activate ds
```

すでに `ds` 環境を作成済みの場合は、

```bash
conda activate ds
```

だけで構いません。

## Clone this repository

このリポジトリは公開リポジトリです。

GitHubアカウントを持っていなくても、HTTPSを使って自分のPCにcloneできます。

```bash
git clone https://github.com/HU-DataScience/ds_advanced.git
```

cloneしたフォルダへ移動します。

```bash
cd ds_advanced
```

VS Codeで開く場合は、

```bash
code .
```

または、VS Codeの

```text
File → Open Folder...
```

から `ds_advanced` フォルダを開いてください。

## Basic workflow

授業では、基本的に次の流れで作業します。

```text
GitHubから教材を取得
        ↓
VS Codeでプロジェクトを開く
        ↓
Python / Jupyter Notebookで作業
        ↓
コードを実行
        ↓
結果を確認
        ↓
Gitで変更内容を確認
        ↓
変更履歴を記録
```

Gitを利用する際は、特に次の流れを意識します。

```text
編集
 ↓
実行・確認
 ↓
git status
 ↓
git diff
 ↓
git add
 ↓
git commit
```

## Git

この授業では、Gitを用いて分析コードやNotebookの変更履歴を管理します。

主に使用するコマンドは次の通りです。

```bash
git status
git diff
git add
git commit
git log
git restore
git clone
```

GitHubとの連携については、授業の進行に合わせて段階的に扱います。

## Google Colab

授業の基本環境は、各自のPC上の

```text
VS Code + Miniforge
```

です。

ただし、以下の場合にはGoogle Colabも利用します。

- ローカル環境の構築に問題がある場合
- 一時的にブラウザ上でPythonを実行したい場合
- GPUを必要とする計算を行う場合

通常のデータ分析およびプロジェクト管理は、VS Code + Miniforge + Gitを基本とします。

## Notes

- 授業ではPython 3.12を使用します。
- Python環境として `ds` を使用します。
- `.py` と `.ipynb` の両方を使用します。
- 大容量データはGitHubに保存しません。
- 個人情報や公開できないデータをGitHubにアップロードしないでください。
- パスワード、APIキー、アクセストークンなどの秘密情報をGitHubに保存しないでください。
- AIが生成したコードを利用する場合も、内容を確認し、実行結果を検証してください。

## Course

**データサイエンス応用 / Data Science Advanced**

Hirosaki University  
HU Data Science


