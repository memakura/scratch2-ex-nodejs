# Node.js を用いた Scratch 2.0 offline の HTTP 拡張ヘルパー

Node.js で新規に Scratch 2.0 オフライン版の拡張を作れます．

## 使い方

詳細は [こちらの記事](https://qiita.com/memakura/items/ca1fff4d7dd33164bb7e#_reference-7d05e075ba7abd791441) を確認してください．

以下，Scratch 2 offline 版が入っているとします．

### 実行形式を使う（Nodeインストール不要）

1. OSに合ったファイルをダウンロードして実行（実行形式ファイルの節を見てください）
1. `s2extest.sb2` をダウンロードして実行

### Nodeがインストールされている

1. コマンドプロンプト（ターミナル）を立ち上げる
1. 以下の順でコマンド実行

    ```
    git clone https://github.com/memakura/scratch2-ex-nodejs.git
    cd scratch2-ex-nodejs
    npm install
    npm test
    ```

### 確認方法

Scratch 2 Offline Editor の「その他」で，赤丸が緑丸になれば立ち上がっています．`beep` でビープ音が鳴ります．
音量が変更できるかようなブロック名ですがダミーです．単にヘルパーと値のをやり取りできるかどうかのテスト用です．

## 実行形式ファイル

ひとまず各プラットフォームで実行可能なバイナリを置きます．

- **Windows** : scratch2-ex-win.exe
- **Mac OS** : scratch2-ex-macos
- **Linux** : scratch2-ex-linux

Windows 以外は未テストです．
なお，プラットフォームのバージョンはデフォルトです．Windows 10 (64bit) + Node.js (v6.11.1) にて zeit/pkg (4.3.0-beta.5) で作成しました．

```
pkg scratch2-ex.js
> pkg@4.3.0-beta.5
> Targets not specified. Assuming:
  node6-linux-x64, node6-macos-x64, node6-win-x64
```
