===================================================
脆弱性対策パッチ 100613
===================================================

1.概要
MODx1.0.3J/1.0.3J-r1で発見された脆弱性を修正するパッチです。
なお、このパッチは日本語版MODxに適用する事が可能です。
(本家版MODxには適用することができません)

2.修正内容

 ・[#MODX-1964] WebLogin does not prevent brute force attack

 ・[#MODX-2009] Clean up handling of 'a' variable in Manager (and related type casting changes)
   ※SQL Injectionになる部分のみ対応
   [参考URL] http://modxcms.com/forums/index.php/topic,50207.0.html

3.パッチ適用方法
srcフォルダ以下のファイルをmodxインストール先の同名フォルダに上書きコピーして
ください。

4.修正対象ソース

 [modxインストール先]/assets/snippets/weblogin/weblogin.processor.inc.php
 [modxインストール先]/manager/includes/accesscontrol.inc.php

5.更新情報
2010/06/13 … リリース
