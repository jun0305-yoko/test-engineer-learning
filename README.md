# test-engineer-learning

このリポジトリはテストデータ作成やテスト自動化の学習用リポジトリです。

## 概要
- テストデータ（サンプルExcelなど）を生成・管理し、pytestで自動テストを実行するためのサンプルを置きます。

## 必要環境
- Python 3.10+（プロジェクトで使用するバージョンに合わせてください）
- pip

## セットアップ
1. リポジトリをクローン

   git clone https://github.com/jun0305-yoko/test-engineer-learning.git
   cd test-engineer-learning

2. 仮想環境を作成して有効化

- macOS/Linux

   python3 -m venv .venv
   source .venv/bin/activate

- Windows (PowerShell)

   python -m venv .venv
   .\.venv\Scripts\Activate.ps1

3. 依存関係をインストール

   pip install -r requirements.txt

（requirements.txt がない場合は、必要なパッケージを直接インストールしてください。例: pip install pandas openpyxl pytest）

## テストデータの生成
- テスト用データを生成するスクリプト（例: data/generate_sample.py）がある場合は、テスト実行前にそれを実行して sample.xlsx を生成してください。例:

   python data/generate_sample.py

## テストの実行

   pytest -q

## 開発フロー
- VS Code を使う場合は、Microsoft の Python 拡張を入れて、インタプリタにプロジェクトの仮想環境（.venv）を指定してください。
- テストは pytest を使っており、GitHub Actions を導入すれば PR ごとに自動でテストが走るようにできます。

## 貢献
- Issue / PR を歓迎します。まずは簡単な README の改善、テストケースの追加、テストデータ生成スクリプトの追加などから始めてください。

---

（このREADMEはリポジトリに直接作成しました。内容を修正したければ編集しますので、追加で記載したい情報を教えてください。）
