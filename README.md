# PPMS-Analysis
PPMS の ρ-T, Hall 測定を解析及びプロットする

## VSCode上での Python 環境構築

1. Python インストール  
   [Python公式サイト](https://www.python.org/downloads/)から最新版のPythonをダウンロードし、インストールします。  
   インストール時に「Add Python to PATH」にチェックを入れることを忘れないでください。

2. VSCode インストール
    [Visual Studio Code公式サイト](https://code.visualstudio.com/)からVSCodeをダウンロードし、インストールします。

3. Python 拡張機能のインストール  
   VSCodeを起動し、左側の拡張機能アイコンをクリックします。  
   検索バーに「Python」と入力し、Microsoftが提供するPython拡張機能をインストールします。

## このリポジトリのクローン
まず, このリポジトリを作成したいディレクトリでターミナルを開きます。
ターミナルを開き、以下のコマンドを実行してこのリポジトリをクローンします。

```bash
git clone https://github.com/Yoshimi-Lab/PPMS-Analysis.git
```

## 仮想環境の構築
Pythonの仮想環境を作成し、必要なパッケージをインストールします。

### venv を用いる場合

VSCode でリポジトリを開き、ターミナルを開いて以下のコマンドを実行します。

#### リポジトリの開き方

VSCodeを起動し、「ファイル」→「フォルダーを開く」を選択し、クローンしたリポジトリのフォルダを選択します。

VSCode のターミナルで以下のコマンドを実行して仮想環境を作成します。

```bash
$ ...\PPMS-Analysis > python -m venv venv
```
次に、仮想環境をアクティブにします。
- Windows:
```bash
PPMS-Analysis .\venv\Scripts\activate
```
- macOS/Linux:
```bash
PPMS-Analysis source ./venv/bin/activate
```
仮想環境がアクティブになったら、必要なパッケージをインストールします。

```bash
PPMS-Analysis pip install -r requirements.txt
```

### uv を用いる場合
`uv`コマンドラインツールを使用して仮想環境を管理する場合

```bash
$ ...\PPMS-Analysis > uv sync
```
## 仮想環境の選択

VSCodeで仮想環境上でPythonを実行するには, .pyファイルでは右下のインタープリターの選択から作成したvenvを選択してください.
.ipynbファイルでは右上のカーネルの選択から作成したvenvを選択してください.

## 使い方
`example.ipynb`を開き、セルを順番に実行して解析とプロットの方法を確認してください。