===================================================
脆弱性対策パッチ 100512
===================================================

1.概要
MODx1.0.2Jで発見された脆弱性を修正するパッチです。
なお、このパッチは日本語版MODxに適用する事が可能です。
(本家リリース版に適用すると英文だった一部メッセージが日本語に変わります)

2.修正内容

 ・XSS possibilities with the SearchHighlight plugin (used by AjaxSearch) as 
   reported in JVN#19774883 and JVN#46669729
 ・Unwanted information disclosure about the site structure in the TinyMCE 
   plugin
 ・SQL Injection via WebLogin

 [参考URL] http://modxcms.com/forums/index.php/topic,47759.msg280304.html#msg280304

3.パッチ適用方法
パッチの適用は次の2パターンがあります。

3.1新規でMODxのインストールから始める場合
srcフォルダ以下のファイルをmodxインストール先の同名フォルダに上書きコピーした
後にMODxのインストールを始めてください。

3.2稼動中のMODxへ適用する場合
srcフォルダ以下(/installフォルダを除く)をMODxインストール先の同名フォルダに
上書きコピーしてください。
/install直下にあるplugin.searchhighlight.tplの中身をSearch Highlightプラグイン
のプラグインコードに上書きしてください。
(MODx管理画面->エレメント->エレメント管理->プラグイン->Search Highlight)

4.修正対象ソース

 [modxインストール先]/assets/plugins/tinymce/tinymce.linklist.flat.php
 [modxインストール先]/assets/plugins/tinymce/tinymce.linklist.php
 [modxインストール先]/assets/snippets/ajaxSearch/plugin.advSearchHighlight.tpl
 [modxインストール先]/assets/snippets/ajaxSearch/plugin.searchHighlight.tpl
 [modxインストール先]/assets/snippets/weblogin/weblogin.inc.php
 [modxインストール先]/install/assets/plugins/searchhighlight.tpl

5.更新情報
2010/05/12 … リリース
