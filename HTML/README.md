# HTMLのチュートリアル

## 概要
WebPage1は、HTMLのチュートリアルです。\
以下のチュートリアルを参考にしています。\
https://github.com/free-honda/HTML-Tutorial

## HTML

### タグ

- 見出し `<h1>`
- 段落 `<p>`  
- 改行 `<br>`
- 画像 `<img=[URL or Dir] alt="[テキスト]">`

## Git

### 直近のコミットメッセージの変更

```git
git commit --amend -m "変更したいメッセージ"
```

### コミットメッセージの書き方

可能であれば、プレフィックスを以下のように統一する。

- feat : 機能追加
- fix : バグ修正
- refactor : リファクタリング
- test : テスト関連
- build : ビルド、補助ツール
- lib : ライブラリ関連
- docs : ドキュメント変更(README.mdなど)

### n個前のコミットメッセージの変更

- リベース

    ```git
    git rebase -i HEAD~n
    ```

- vimが開かれるの`i`でINSERTモードへ
- 修正したいコミットメッセージの`pick`を`edit`に変更
- `esp` + `:wq`でvimの変更内容を保存して終了

- コミットメッセージの変更

    ```git
    git commit --amend -m "変更したいメッセージ"
    ```

- 最新のコミットに戻る

    ```git
    git rebase --continue
    ```

## 参考

- https://qiita.com/konatsu_p/items/dfe199ebe3a7d2010b3e
- https://qiita.com/kenose0328/items/185f7e8634d816c85a84