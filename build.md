git clone https://github.com/tztechno/vercel_hugo.git

git clone https://github.com/tztechno/vercel_hugo.git

cd vercel_hugo
git init
git remote add origin https://github.com/tztechno/vercel_hugo
git pull
git add .
git commit -m "2024-07-20"
git push -u origin main

git push -f origin main

cd vercel_hugo




---

VercelのテンプレートからHugoサイトをデプロイした場合、以下の手順で記事を追加できます：

1. ローカルにリポジトリをクローン:
   ```
   git clone <your-github-repo-url>
   ```

2. 新しい記事を追加:
   Hugoの`content`ディレクトリに新しいMarkdownファイルを作成します。
   ```
   touch posts/my-new-post.md
   hugo new posts/my-new-post.md
   ```

3. 記事を編集:
   作成したMarkdownファイルを編集し、内容を追加します。

4. ローカルでサイトをプレビュー（オプション）:
   ```
   hugo server
   ```

5. 変更をコミットしてプッシュ:
   ```
   git add .
   git commit -m "Add new post"
   git push origin main
   ```

6. Vercelがデプロイを自動的に処理:
   GitHubにプッシュすると、VercelがHugoサイトを自動的にビルドしデプロイします。

重要なポイント:
- 別のリポジトリにプッシュする必要はありません。
- Vercelは自動的にHugoコマンドを実行し、静的HTMLを生成します。
- ローカルでHTMLを生成する必要はありません。

Vercelの設定で、ビルドコマンドとアウトプットディレクトリが正しく設定されていることを確認してください：

- ビルドコマンド: `hugo --gc --minify`
- アウトプットディレクトリ: `public`

これらの手順に従えば、GitHubリポジトリに変更をプッシュするだけで、Vercelが自動的に新しいコンテンツでサイトを更新します。

追加の情報や特定の部分について詳しく知りたい場合は、お知らせください。
