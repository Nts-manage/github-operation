# GitHub でのリポジトリ管理

## Organization を作成する
新しくプロジェクトを作り、リポジトリをグループでまとめるときは Organization を作成する。

1. 右上のユーザーアイコンをクリックする。
![](./images/make-org0.png)


2. [Your organizations] を選択する。
![](./images/make-org1.png)

3. [New organization] を選択する。
![](./images/make-org2.png)

4. 以下を入力する
   * 組織名
   * 責任者のメールアドレス
   * 所属: My personal account 
![](./images/make-org3.png)


## Organization へユーザーを追加する
※ 事前に個別メンバーのGitHubアカウントを作っておいたほうが楽になる。

1. [People] を選択する。
![](./images/add-member0.png)

2. [Invite member] を選択する。
![](./images/add-member1.png)


3. 招待するユーザーのGitHubアカウント名、またはメールアドレスを入力して [Invite] をクリックする。
![](./images/add-member2.png)

4. 権限を選ぶ
mainブランチへのマージを行う人は Owner 、それ以外は Member を選択する。
![](./images/add-member3.png)

※ メンバーの権限は後から変更できる。
![](./images/add-member4.png)

5. メンバーに招待メールが届くのでリンクから参加する。


## リポジトリを作成する
割愛


## 自分のアカウントにSSHキーを登録する
1. ユーザーアイコンのメニューから [Settings] を選択する。
![](./images/ssh-key0.png)

2. [SSH and GPG keys] を選択する。
![](./images/ssh-key1.png)

3. [New SSH key] をクリックする。
![](./images/ssh-key2.png)

4. 以下の情報を入力して登録する。
   * Titile: 任意の名前
   * Key type: Authentication key
   * Key: SSH公開鍵の内容
![](./images/ssh-key3.png)

SSH公開鍵を作成していない場合は、次の手順で作成する。

### SSHキーペアを生成する

1. Windows Powershell を開き、`ssh-keygen` コマンドを入力する。途中で聞かれる質問はすべてEnterで返してよい。
![](./images/ssh-keygen.png)

2. SSH公開鍵および秘密鍵はデフォルトでは `C:/Users/(username)/.ssh/` に作成される。
   * 秘密鍵: `id_rsa`
   * 公開鍵: `id_rsa.pub`  <- こちらをGitHubへ登録
