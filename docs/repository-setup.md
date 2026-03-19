# レポジトリの新規作成と移動

1. [はじめに](#anchor1)
1. [新しくリポジトリを作成する](#anchor2)
1. [既存のリポジトリを移動する](#anchor3)

---

<a id="anchor1"></a>
## 1. はじめに
GitHubはプログラムのソースコードをオンライン上に保存/管理したり、チームで共有/共同開発するためのプラットフォームです。GitHubリポジトリはGitHub上に各プロジェクトのソースコードやその編集履歴を保存/管理するための場所です。

> リポジトリには、すべてのコード、ファイル、および各ファイルのリビジョン履歴が含まれています。リポジトリ内で作業についてディスカッションをしたり、作業を管理したりできます。<br>
出典: https://docs.github.com/ja

このOrganizationで開発を行う際は、以下のような方法でリポジトリを用意してください。

---

<a id="anchor2"></a>
## 2. 新しくリポジトリを作成する
### リポジトリの作成
まずは、GitHub上にプロジェクトのソースコードとその編集履歴を保存するためのGitHubリポジトリを作成します。
1. Organizationの[Repositoriesページ](https://github.com/orgs/KUN-Command-Team/repositories)にアクセスし右上の [New repository] ボタンをクリックします。<br>
   <img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/b7ee6ff9-187d-4684-818e-4ee1a3402187" />
1. Owner が **KUN-Command-Team** になっていることを確認したのち、必要事項を入力し [Continue: Configuration] ボタンをクリックします。
1. Configurationでは [Choose visibility] から 公開 / 非公開 の設定を行います。`Private`に設定した場合、リポジトリはメンバーだけが閲覧できます。一方で、`Public`に設定されたリポジトリはURLを知っている人全員が閲覧できるようになります。
1. README, .gitignore, LICENCEについては後ほど設定するのでとりあえず、無視して構いません。
1. [Create repository] をクリックして完了です。

### プロジェクトのプッシュ
GitHubリポジトリが作成出来たら、次に作業しているコンピュータ上のローカルリポジトリとリモートリポジトリを紐づける必要があります。Gitがインストールされていない場合、[https://gitforwindows.org](https://gitforwindows.org) からインストーラをダウンロードしてインストールしてください。

ローカルリポジトリを作成するためには、アップロードしたいプロジェクトのルートディレクトリに移動したのちに以下のコマンドを実行します。これらのコマンドでは、ローカルリポジトリを作成し、すべてのファイルをステージングした後に、現在のブランチ名を main に変更しています。

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
```

ローカルリポジトリは以下のようなコマンドでリモートリポジトリと紐づけることができます。

```bash
git remote add origin <リポジトリのURL>
```

これでローカルリポジトリとリモートリポジトリを関連付けることができました。次に以下のコマンドを実行してmainブランチをリモートリポジトリにプッシュします。

```bash
git push -u origin main
```

### Git GUIツール？
Git GUIツールを使うことでより直感的にGitを操作できます。

また、VSCodeのソース管理タブなどからもGUI上でGitの操作を行えます。

---

<a id="anchor3"></a>
## 3. 既存のリポジトリを移動する
自分のアカウントで既に管理しているリポジトリを Organization に移動します。この操作は KUN-Command-Team のメンバーになってから行ってください。
1. 管理しているGitHubリポジトリの [Settings] ページへ移動します。<br>
   <img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/928d4f22-eaea-473b-96e1-7af0d1b1ab20" />
1. 下へスクロールして Danger Zone内にある [Transfer] ボタンを見つけクリックします。<br>
   <img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/5aaada12-7ec4-4529-b687-53abcf854a2a" />
1. New owner が **KUN-Command-Team** になっていることを確認したのち、必要事項を入力してください。<br>
   <img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/0356142e-3ccb-4c1d-86ef-6c7a37f7ea0c" />
1. レポジトリ名を入力したのち、 [I understand, transfer this repository.] ボタンをクリックして完了です。<br>
   <img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/56d0d2be-1e27-4ffe-b8c9-c91135234cd5" />
