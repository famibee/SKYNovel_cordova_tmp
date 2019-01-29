# SKYNovel_cordova_tmp
SKYNovel cordova template

[![Apache License](https://img.shields.io/github/license/famibee/SKYNovel_cordova_tmp.svg)](LICENSE)
![](https://img.shields.io/badge/platform-Android%20%7C%20iOS-lightgrey.svg)

![logo.svg](https://github.com/famibee/SKYNovel/blob/master/test/icon.svg)

[CHANGELOG.md](CHANGELOG.md)

## usage（使用法）

### インストールと環境設定
 1. （PC版のプロジェクトフォルダ）で「フォルダを開く」したVSCodeのターミナルで以下のコマンドを入力していく。
	- あるいはコマンドラインやターミナルで、cd （PC版のプロジェクトフォルダ）
 2. cordova create mobile com.fc2.blog.famibee.skynovel.（何かいい感じに他の制作者と区別できそうな英文字とピリオドによるID名） ゲームタイトル名 --template https://git@github.com:famibee/SKYNovel_cordova_tmp.git
 3. ln -s prj mobile/www
 4. （Android版を作りたいなら）cordova platform add android
 5. （iOS版を・も作りたいなら）cordova platform add ios
	- 後で削除・再度追加も自由に出来ます。詳細は上記コマンドで検索。
 6. cordova requirements で、問題がありそうな表示が出ないか確認。ダメっぽい項目はメッセージを検索しては直していく。ここが一番大変。
 7. VSCodeやテキストエディタで「config.xml」「package.json」を変更（項目の意味は cordova について検索）

### 普段の開発
 1. PC版のプロジェクトフォルダで「フォルダを開く」したVSCodeでタスク「webpack:dev:w」を実行し、index.jsを生成。
 2. ｘ【AND:Dev】タスクを実行
	- （既知の問題）package.jsonの【scripts】【AND:Dev】タスクの中身を、直接ターミナルで実行して下さい。
 3. デバッグ（ざっくり云うとconsole.log()の表示が見える、ということ）については、こちらの記事が参考になります。
	- [３分間でiOS、Android両対応アプリを作る - Qiita](https://qiita.com/teradonburi/items/5b214c74cddd776cb67f)
