# GitHubでローカルリポジトリを作成する手順

## 1. 新しいディレクトリを作成
ターミナルで作業ディレクトリを作り、移動する。

```
mkdir my_project
cd my_project
```

## 2. Gitを初期化する
```
git init
```

## 3. ファイルを作成し、Gitに追加する
```
echo "# My Project" > README.md
git add .
git commit -m "initial commit"
```

## 4. GitHubにリポジトリを作成
1. GitHubにログイン
2. New Repositoryを作成
3. リポジトリ名を決め、Create Repositoryをクリック

## 5. GitHubのリポジトリとローカルを接続
GitHubで表示されるリポジトリのURLを使って、リモートを追加
```
git remote add origin https://github.com/username/my_project.git
```

## 6. GitHubにプッシュする
```
git branch -M main  # ブランチ名を main に変更（デフォルトが master の場合）
git push -u origin main  # GitHubに最初のプッシュ
```

## 7. 変更を加えた時の更新手順
1. ファイルを変更
2. ステージング
```
git add .
```
3. コミット
```
git commit -m "update some files"
```

4. GitHubにプッシュ
```
git push origin main
```

## 8. GitHubリポジトリをローカルにクローン
```
git clone https://github.com/username/my_project.git
```