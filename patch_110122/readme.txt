===================================================
脆弱性対策パッチ 110122
===================================================

1.概要
MODx1.0.5Jより以前のバージョンに発見された脆弱性を修正するパッチです。
なお、このパッチは日本語版MODxに適用する事が可能です。

2.修正内容

 ・[#3437] fix vulnerability in AjaxSearch allowing attacker to view arbitrary files (JVN#95385972)
   対象MODxバージョン：1.0.4J-r5 〜 1.0.3Jr2

 ・[#3429] fix SQL injection vulnerability in AjaxSearch allowing attacker to execute arbitrary PHP code (JVN#54092716)
   対象MODxバージョン：1.0.4J-r5 〜 1.0.3Jr2

3.パッチ適用方法
srcフォルダ以下のファイルをmodxインストール先の同名フォルダに上書きコピーして
ください。

4.修正対象ソース

 [modxインストール先]/assets/snippets/ajaxSearch/classes/ajaxSearchOutput.class.inc.php
 [modxインストール先]/assets/snippets/ajaxSearch/classes/asPhxParser.class.inc.php

5.更新情報
2011/01/22 … リリース
