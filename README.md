# Sublime_Text_2
自分のSublime Text 2の設定ファイル群

http://blog.manaten.net/entry/sublimetext-git  
このへんを参考にしました。

実際にはPackages/User配下の一部ファイルだけでいいらしいけど面倒なのでApplication Support/Sublime Text 2をまるごと管理。
しかし以下は管理しない。

- .sublime_licence
- .DS_Store
- Backupディレクトリ  

Sublime Text 3でも同様にApplication Support/Sublime Text 3を管理すればいいだけのはず。

## Application Supportの場所は？
Mac OSX 10.8以降？ではユーザーのLibraryディレクトリは見えなくなっているので以下の方法で移動する。

### Finder画面上部の「移動」
移動メニューを「Option」を押しながらクリックすると「ライブラリ」メニューが出でるのでそれをクリック。

### Application Supportを探す
ライブラリに移動したら、Application Supportへ移動します。
Mac OSXでは、インストールされているアプリケーションのさまざまな設定ファイルがApplication Supportに格納される仕様になっています。
このディレクトリ配下のファイルを消したりすると、そのアプリケーションの設定がすっとぶのでご注意。

よーくさがすとSublime Text 2というフォルダが有るはずです。
