## GitHub リポジトリの変更プロセス

### 既にクローンしている場合
#### 1. 最新の変更を取得
'''bash
cd OR  
git checkout main  
git pull origin main  
'''

```bash
git clone https://github.com/itomond-home/OR.git
cd OR
git checkout -b new-feature
```

#### 2. 新しいブランチの作成
'''
 git checkout -b new-feature
'''

以降の手順（3. コードの追記、4. 変更のステージング、5. コミットの作成、6. GitHubにプッシュ、7. プルリクエストの作成）は「初めてクローンする場合」と同じ。

### 新規クローンからの変更プロセス
#### 1.リポジトリのクローン
ローカルマシンにリポジトリをクローンします。
'''
 git clone https://github.com/itomond-home/OR.git
'''

#### 2.ブランチの作成
作業用の新しいブランチを作成します。

'''
 cd OR
 git checkout -b new-feature
'''

#### 3.コードの追記
必要な変更をファイルに加えて保存します。

#### 4.変更のステージング
すべての変更をステージングします。
'''
 git add .
'''

※特定のファイルのみをステージングする場合は、ファイル名を指定します。
'''
 git add <ファイル名>
'''

#### 5.コミットの作成
ステージングされた変更をコミットします。
'''
 git commit -m "新しい機能を追加"
'''

#### 6.GitHubにプッシュ
ローカルのブランチをGitHubにプッシュします。

'''
git push origin new-feature
'''

#### 7.プルリクエストの作成
GitHubのウェブサイトで、new-featureブランチからmainブランチへのプルリクエストを作成します。
