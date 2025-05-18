# GitHubでリポジトリを公開する手順

このプロジェクトをGitHubで公開するための手順は以下の通りです。

## 1. GitHubでリポジトリを作成

1. GitHub（https://github.com）にアクセスし、ログインします。
2. 右上の「+」ボタンをクリックし、「New repository」を選択します。
3. 以下の情報を入力します：
   - Repository name: `dinner-preparation-agent`（または希望の名前）
   - Description: 「AI支援による夕食準備プロセスを自動化するCursor AI用ルールとサンプル」
   - Visibility: Public
   - Initialize this repository with: README（チェックしない）
4. 「Create repository」ボタンをクリックします。

## 2. ローカルリポジトリをGitHubに接続

GitHubリポジトリ作成後、表示される指示に従って以下のコマンドを実行します：

```bash
# リモートリポジトリを追加（URLは実際に作成したリポジトリのURLに置き換えてください）
git remote add origin https://github.com/yourusername/dinner-preparation-agent.git

# メインブランチをプッシュ
git push -u origin main
```

## 3. READMEのリンク修正

リポジトリ公開後、READMEファイル内のリポジトリURLを正しいものに更新します：

1. `README.md`ファイルを開きます。
2. ブログコンテンツ内の「リポジトリ: github.com/yourusername/dinner-preparation-agent」を実際のリポジトリURLに更新します。
3. 変更をコミットしてプッシュします：

```bash
git add README.md blog_content.md
git commit -m "リポジトリURLを更新"
git push
```

## 4. 公開確認

GitHubで自分のリポジトリページにアクセスし、すべてのファイルが正しくアップロードされていることを確認します。

## 5. ブログ記事との連携

ブログ記事内で、このリポジトリへの参照を追加します。具体的には：

1. `blog_content.md`の内容をブログプラットフォームにコピー
2. 記事内の「リポジトリ」リンクを実際のGitHubリポジトリURLに更新
3. 必要に応じて、興味深いコードスニペットへの直接リンクを追加

## 6. ブログでのリポジトリの紹介方法

以下のようなポイントを強調するとよいでしょう：

1. **リポジトリの目的**: 日常タスクをAIで自動化する実験的プロジェクトであること
2. **技術的なポイント**: Cursor AIのルール機能を活用した独自エージェントの作成方法
3. **カスタマイズの可能性**: 読者が自分のニーズに合わせてプロジェクトを拡張できること
4. **コントリビューションの歓迎**: 改善提案やPull Requestを歓迎すること 