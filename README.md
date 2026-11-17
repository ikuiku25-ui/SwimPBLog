[README.md](https://github.com/user-attachments/files/34948611/README.md)
# SwimPBLog（iPhone版）GitHub Pages 用

競泳の自己ベスト・ラップ管理ツールの、結果取り込み専用iPhone版です。
データはiPhoneのブラウザ内（localStorage）にだけ保存され、このリポジトリには入りません。
PC版とのデータのやり取りは、JSONの書き出し／読み込みで行います。

## 入っているファイル

| ファイル | 内容 |
|---|---|
| swimpblog.html | 本体（結果の取り込みアプリ） |
| index.html | 入口（開くと自動で本体へ移動します） |

## 公開の手順（10分ほど）

1. GitHubにログインし、新しいリポジトリを作る
   - 名前は例：`swimpblog`（半角英数字）
   - **Public** を選ぶ（無料プランのGitHub Pagesは公開リポジトリが前提）
2. リポジトリの画面で「Add file」→「Upload files」を選び、このフォルダの3ファイルをアップロードして「Commit changes」
3. リポジトリの「Settings」→ 左メニューの「Pages」
4. 「Build and deployment」の Branch を **main / (root)** にして「Save」
5. 数分待つと、Pagesの画面に公開URLが表示される
   - 形：`https://（ユーザー名）.github.io/swimpblog/`
6. iPhoneのSafariで公開URLを開き、「共有」→「ホーム画面に追加」
   - ホーム画面の名前は「SwimPBLog」になります

## データについて

- 保存データはURLごとに分かれます。公開URLで使い始めたら、以後はずっと同じURLで開いてください。
- 一時リンクで試したときのデータは、新しいURLでは見えません（試用データとして割り切ってください）。
- PC版から選手・ベストを引き継ぐときは、PC版でJSONを書き出し、SwimPBLogの「設定」タブで読み込みます。逆も同じです。

## 更新のしかた

- 新しい版ができたら、リポジトリで `swimpblog.html` を同じ名前のままアップロードし直すだけです。URLは変わらないので、保存データはそのまま使えます。
- ファイル名は変えないでください。名前が変わると別のURLになり、データが見えなくなります。
