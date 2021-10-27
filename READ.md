# laravelSailでTodoアプリを作る

## [Laravel Sail](https://readouble.com/laravel/8.x/ja/installation.html#your-first-laravel-project)（Laravel公式Docker環境）

1.下記curlコマンドを叩く
`curl -s "https://laravel.build/{アプリ名}" | bash`

    - 上記コマンドにクエリを付け足すとsailサービス選択することができる。
    - サービス指定をしない場合、下記サービスがデフォルト
        - mysql
        - redis
        - meilisearch
        - mailhog
        - selenium

2.sail開始と停止
    - Sailコマンドは`vendor/bin/sail`スクリプトを使用して起動している
        - 繰り返し入力するの怠いので、Bashエイリアスを設定しておくと`sail`と入力するだけでSailコマンド実行できて便利
        `alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'`
    - Sailの開始
    `sail up -d`
    - Sailの停止
    `sail stop`

3.