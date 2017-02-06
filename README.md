# My bash on ubuntu on window

## uninstall/install

* cmdから以下のコマンドで実行できる
 * install : `lxrun /uninstall`
 * install : `lxrun /install`

## Terminal software
日本語がちゃんと表示できる
* ここからDL
 * https://github.com/goreliu/wsl-terminal/releases

## ansibleインストールまでの手動初期設定

* デフォルトエディタをvimに変更
`sudo update-alternatives --config editor`
* ansible実行ユーザはNOPAAWD化
`sudo visudo`
以下の行を追加
```
[ansible実行ユーザ名] ALL:NOPASSWD: ALL
```

* ANSIBLEをインストール
```
sudo apt-add-repository ppa:ansible/ansible
sudo apt update
sudo apt install ansible
```

* gitインストール
```
sudo apt install git
```

これ以降はansibleでセットアップ

