# レポジトリの検索と整理

1. [はじめに](#anchor1)
1. [Topics](#anchor2)
1. [Custom properties](#anchor3)

---

<a id="anchor1"></a>
## 1. はじめに
Organization内のレポジトリは、 [https://github.com/orgs/KUN-Command-Team/repositories](https://github.com/orgs/KUN-Command-Team/repositories) から探すことができます。来訪者がレポジトリを探しやすくするために、開発者は以下のような工夫をすることができます。

---


<a id="anchor2"></a>
## 2. Topics
リポジトリにタグを付けて分類・検索しやすくするための機能です。

> あなたのプロジェクトを他の人が見つけて貢献しやすくするために、プロジェクトの目的、分野、主催グループなどの、リポジトリに関するトピックを追加できます。<br>
出典：https://docs.github.com/ja

<img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/d1a2f5e8-a93b-4ddf-b083-4a3efc93b7ac" />

### Topicの付け方
1. レポジトリの右上にある [歯車アイコン] をクリックする。
1. Topicsに半角スペース区切りでTopicを入力する。

### Topicの例:
| Topic | 説明 | 具体例 |
| :-- | :-- | :-- |
| `utility` | 汎用的な機能追加MOD | UI改善、共通機能追加など |
| `tools` | 開発・運用を補助するMOD | デバッグ、管理コマンド、開発支援機能など |
| `library` | --- | API提供、前提MOD、依存ライブラリなど |
| `bugfix` | バグを直接修正するMOD | --- |
| `workaround` | バグの回避策を提供するMOD | 問題機能の無効化・代替処理など |
| `benchmark` | 性能測定・検証用MOD | TPS測定、処理負荷の比較・可視化など |


---


<a id="anchor3"></a>
## 3. Custom properties
リポジトリに構造化されたキーと値を付与して管理する機能です。Topicsと異なり、あらかじめ定義された項目に従って値を設定します。

> カスタム プロパティは構造化されたメタデータ フィールドであり、GitHub のリポジトリと組織に追加して、環境全体の組織、ガバナンス、自動化を向上させることができます。<br>
出典：https://docs.github.com/ja

<img width="674" height="388" alt="image" src="https://github.com/user-attachments/assets/6ffa245e-72eb-49ec-a824-a56d2c3ef53d" />

### Custom propertiesの付け方
1. 管理しているGitHubリポジトリの [Settings] ページへ移動します。
1. 左のタブから [Custom properties] を探して開きます。
1. それぞれのタグを入力します。
