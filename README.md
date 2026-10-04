# Data Science Advanced

弘前大学「データサイエンス応用B」で使用する教材配布用リポジトリです。

この授業では、Pythonによるデータ分析・統計・機械学習を学びます。
第7回以降は GitHub Copilot も利用し、生成されたコードを読んで理解しながら分析を進めます。

Git / GitHub は学習対象ではなく、教材の配布・更新に使用します。

## Course objectives

この授業では、以下の能力を身につけることを目標とします。

- VS Code と Miniforge を用いて Python 実行環境を構築する
- Python コードを読んで、処理内容を理解する
- pandas、Matplotlib などを用いてデータを分析する
- 統計・機械学習の基本的な考え方を理解する
- Jupyter Notebook を用いてデータ分析を実行する
- AIによるコーディング支援を利用し、生成されたコードを確認・検証する
- 分析結果を解釈し、次に何を調べるべきか判断する

## Repository structure
```
ds_advanced/
├── README.md
├── environment.yml
├── data/          # 授業で使用するデータ
├── src/           # 補助的なPythonコード
├── notebooks/     # Live演習用Notebook
└── quiz/          # Moodleから配布される小テスト用ファイル
```

### data

授業で使用するデータを置きます。

### src

Notebookから利用する補助的なPythonコードを置きます。

### notebooks

第7回以降のLive演習で使用するJupyter Notebookを置きます。

GitHubから取得したNotebookは原本として残し、
授業では別名でコピーして実行・編集します。

### quiz

小テスト用の作業フォルダです。

小テスト開始時に Moodle から配布されたファイルをダウンロードし、
このフォルダに移動して実行します。

quiz/ 内の提出用ファイルは Git の管理対象外です。

## GitHubの使い方

### 第2回

初回のみ GitHub から教材を取得します。

git clone https://github.com/HU-DataScience/ds_advanced.git

### 第3回〜第6回

Python基礎は Moodle 教材を使用します。

小テストは Moodle からダウンロードし、
quiz/ に移動して実行します。

### 第7回以降

授業開始時に教材を最新版へ更新します。

cd ~/Documents/ds_python/ds_advanced
git pull

Live演習では notebooks/ のNotebookを使用します。

小テストは第3回以降と同様に、
Moodleからダウンロードして quiz/ で実行します。

## Python environment

この授業では Miniforge を利用し、
授業用環境 ds を使用します。

conda activate ds

Python 3.12 を使用します。

必要に応じて environment.yml から環境を作成できます。

conda env create -f environment.yml
