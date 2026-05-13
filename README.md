# 株式会社YUYU コーポレートサイト

株式会社YUYUの公式コーポレートサイトプロジェクトです。
清潔感と信頼感を重視した、モダンでレスポンシブなデザインを採用しています。

## 構成
- **HTML5**: セマンティックなマークアップ
- **Tailwind CSS**: ユーティリティファーストなスタイリング
- **AOS (Animate On Scroll)**: スクロールアニメーション
- **Lucide Icons**: シンプルで洗練されたアイコン

## ディレクトリ構成
```text
YUYU/
├── index.html        # メインのランディングページ
├── assets/           # 画像、ロゴなどのアセット
│   ├── logo.png      # 企業ロゴ
│   └── hero.png      # メインビジュアル
└── README.md         # プロジェクト説明・デプロイ手順
```

## デプロイ手順

### 1. GitHubへのプッシュ
1. GitHubで新しいリポジトリを作成します（例: `yuyu-corp-site`）。
2. ローカル環境で以下のコマンドを実行します：
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Create corporate site"
   git branch -M main
   git remote add origin https://github.com/あなたのユーザー名/yuyu-corp-site.git
   git push -u origin main
   ```

### 2. Cloudflare Pagesでの公開
1. [Cloudflare ダッシュボード](https://dash.cloudflare.com/)にログインします。
2. 「Workers & Pages」 > 「作成」 > 「Pages」を選択します。
3. 「Git に接続」をクリックし、先ほど作成したリポジトリを選択します。
4. 設定画面で以下を確認します：
   - **プロジェクト名**: `yuyu-corp`（任意）
   - **プロダクションブランチ**: `main`
   - **フレームワーク プリセット**: `None` (静的サイトのため)
   - **ビルドコマンド**: (空欄のまま)
   - **ビルド出力ディレクトリ**: `.` (ルートディレクトリ)
5. 「保存してデプロイ」をクリックします。
6. 数分で `https://yuyu-corp.pages.dev` のようなURLで公開されます。

---
Developed by Antigravity
