# TANKORE - 英単語帳アプリ

TANKOREは、自分だけのオリジナル英単語帳を作成できるWebアプリケーションです。

## 機能

###  ユーザー認証
- 会員登録
- ログイン/ログアウト

### 📚# TANKORE - 英単語帳アプリ

TANKORE は、自分用の英単語帳をゆるく作って遊べる Web アプリです。  
覚えたい単語だけ集めたり、他の人の単語帳をのぞいたりできます。

## なにができるか

- 会員登録してログイン / ログアウト
- 単語帳の作成・編集・削除
- 自分の単語帳と、他のユーザーの単語帳を分けて表示
- 人気の単語帳や、みんなが作った単語帳を参考にできる
- 単語カード（単語＋意味）をどんどん追加
- 画像も付けられるので、ビジュアルで覚えたい人向け

見た目はピンク系のかわいい UI で、スマホでも普通に使えます。

## ざっくり技術スタック

- Backend: Django 5.2.7
- Frontend: HTML / CSS / JavaScript
- Database: SQLite（開発用）
- Language: Python 3.13

## セットアップ方法

Python と pip が入っている前提です。

1. リポジトリをクローンする

   ```bash
   git clone <repository-url>
   cd django
   ```

2. 仮想環境を作る（任意）

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # macOS / Linux
   # Windows の場合:
   .venv\Scripts\activate
   ```

3. 必要なパッケージを入れる

   ```bash
   pip install Django Pillow
   ```

4. マイグレーションする

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. サンプルデータを入れたい場合（任意）

   ```bash
   python manage.py create_sample_data
   ```

6. 開発サーバーを起動

   ```bash
   python manage.py runserver
   ```

ブラウザで `http://127.0.0.1:8000/` を開けば動作確認できます。

## ざっくり使い方

1. トップページから新規登録してログイン
2. 自分の単語帳を作って単語カードを追加
3. 他の人の単語帳も見ながら、覚えたい単語を増やしていく

細かい機能は画面を触りながら確認してもらう想定です。 単語帳管理
- 単語帳の作成・編集・削除
- 自分の単語帳と他のユーザーの単語帳を分けて表示
- 人気の単語帳や既存の単語帳を参照

### 📝 単語カード機能
- 単語カードの追加・削除
- 英単語と意味の記録
- 画像の添付（視覚的学習をサポート）

### 🎨 デザイン
- ピンク系の可愛らしいUI
- レスポンシブデザイン（スマホ対応）
- カードレイアウトで見やすい表示

## 技術スタック

- **Backend**: Django 5.2.7
- **Frontend**: HTML5, CSS3, JavaScript
- **Database**: SQLite（開発環境）
- **Language**: Python 3.13

## セットアップ

### 1. リポジトリのクローン
\`\`\`bash
git clone <repository-url>
cd django
\`\`\`

### 2. 仮想環境の作成と有効化
\`\`\`bash
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
# または
.venv\\Scripts\\activate  # Windows
\`\`\`

### 3. 依存関係のインストール
\`\`\`bash
pip install Django Pillow
\`\`\`

### 4. データベースのマイグレーション
\`\`\`bash
python manage.py makemigrations
python manage.py migrate
\`\`\`

### 5. サンプルデータの作成（オプション）
\`\`\`bash
python manage.py create_sample_data
\`\`\`

### 6. 開発サーバーの起動
\`\`\`bash
python manage.py runserver
\`\`\`

サーバーが起動したら、ブラウザで http://127.0.0.1:8000/ にアクセスしてください。

## 使い方

1. **新規登録**: トップページから「今すぐ始める」をクリックして会員登録
2. **単語帳作成**: ログイン後、「+ 新しい単語帳を作成」ボタンから単語帳を作成
3. **単語カード追加**: 作成した単語帳に英単語と意味を追加
4. **学習**: 作成した単語カードを使って学習

## プロジェクト構造

\`\`\`
django/
├── manage.py
├── db.sqlite3
├── myproject/          # プロジェクト設定
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── home/               # メインアプリ
│   ├── models.py       # データモデル
│   ├── views.py        # ビュー（コントローラー）
│   ├── urls.py         # URL設定
│   ├── admin.py        # 管理画面設定
│   ├── templates/      # HTMLテンプレート
│   ├── static/         # 静的ファイル（CSS, JS）
│   └── management/     # カスタムコマンド
└── media/              # アップロードファイル
\`\`\`

## 開発者

@kousei tomita

## ライセンス

このプロジェクトはMITライセンスの下で公開されています。
