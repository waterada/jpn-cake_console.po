jpn-cake_console.po
===================

- CakePHP の `bake` を日本語でできるようにメッセージを日本語化しました。
- これで少しでも `bake` しやすくなれば幸いです。
- CakePHP 2.3 をベースにしています。
- まだ全てを日本語化できていません。随時拡充していきます。


Install
-------

- `cake_console.po` を `app/Locale/jpn/LC_MESSAGES/cake_console.po` に置いてください。
- `lib/Cake/Console/Command/BakeShell.php` を下記のように１行加えてください。

```php
public function startup() {
    Configure::write('Config.language', 'jpn'); //これを追加
    parent::startup();
```

コンソールを日本語化するもっとスマートな方法があると良いのですが。。。
（知ってる人いたら教えてください。）
