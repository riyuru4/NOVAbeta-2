NOVA PWA（アプリ風Webサイト）プロジェクト

これはAPKではなく、ホーム画面に追加してアプリのように起動できるWebサイト用ファイル一式です。

公開方法:
1. ZIPを解凍
2. index.html / manifest.webmanifest / sw.js / icons フォルダを同じ場所関係のままWebサーバーへアップロード
3. HTTPSで公開する（GitHub Pagesなど）
4. AndroidのChromeで公開URLを開く
5. Chromeメニュー ⋮ →「ホーム画面に追加」または「アプリをインストール」

特徴:
- ホーム画面からNOVAを単独画面で起動（対応ブラウザ）
- manifestでアプリ名・アイコン・テーマを設定
- Service WorkerでNOVA本体の基本ファイルをキャッシュ

重要:
- PWA化しても、サイト側がiframe埋め込みを拒否する制限は解除されません。
- このプロジェクトはNOVAのWeb版をアプリ風にするもので、APKを生成するものではありません。
- GitHub PagesなどHTTPS対応の場所で公開する必要があります。
