# NicoNicoCommentScriptHtml5_FireFox&Chrome<br>
<br>
導入:<br>
正式版：<br>
javascript:(function(){var%20s=document.createElement('script');s.src='https://eneko0513.github.io/NicoNicoCommentScriptHtml5_FireFox-Chrome/html5_nico_firefox.js';document.getElementsByTagName('head')[0].appendChild(s);})();

上の文字列をコピーして、FireFoxかChromeのブックマークに追加(URLの部分に上の内容でタイトルは適当に)  
※呼び出そうとしたら検索結果に飛んでしまう場合は、URLの先頭の「javascript:」が消えていないか確認して下さい。  
稀にブラウザによっては、先頭のjavascript:が消されてしまう時があるらしいとのことです。  

使い方:  
1. スクリプトを用いたい動画再生ページ上でブックマークに追加したスクリプトを選択<br>
2. プレイヤー下にテキストエリアとボタンが表示されます  

  説明:
 投下形式:  
 1.1行コメントモードのみ対応 <br>
 example1) <br>
 [コマンド]コメント\<br>コメント[tab]コメント<br>
<br>
 example2) <br>
 [コマンド]コメントコメントコメントコメントコメントコメントコメントコメント
 75文字まで、それ以降はカットされて投稿される<br>
 <br>
 2.自動投下<br>
 上記の1行形式が複数行入力されていれば コメントセット→2秒待機→投下　→　6秒待機　→コメントセット..　を<br>
 コメントがなくなるまで入力を行う入力処理中は他処理を行わない <br>
 3.空行について<br>
 空行がある場合、形式が違いますと表示されてしまうので空行が無い形で投下ボタンを押して下さい<br>
 <br>
 4.どーも形式->1行形式変換<br>
 <br>
 small ue #FFFFFF<br>
 ああああ<br>
 　ああああ<br>
  <br>
 という形式のテキストがあった場合、上のテキストをテキストエリアに追加した状態で変換ボタンを実行すると<br>
 [small ue #FFFFFF]ああああ\<br>　ああああ\<br><br>
 という形式に変換される。その状態でのみ投下が可能。<br>
 ※注意:<br>
 コマンドの最初が サイズ、最後が #カラーコード でないと正常に変換されない<br>
 example)small ue mincho full #ff00ff -> small , #ff00ffでサイズと色が最初と最後についている形式<br>
 ue mincho #ff00ff -> 最初がueなので正常に変換されないので注意<br>
 <br>
 ver0.1 : FireFox&Chrome版とりあえず公開<br>
 ver0.2 : 184投下切り替え機能追加<br>
 ver0.3 : 逆から投下機能追加<br>
 ver0.4 : コマンドに全角文字が含まれていた場合にエラーになる不具合の修正<br>
 ver0.5 : 逆から投下の末尾に改行が存在していた場合にエラーになる不具合の修正<br>
 ver0.6 : 75文字をオーバーしたコメントがある場合はアラートを表示し、コメント投下しない形式に変更<br>
 ver0.7 : 75文字以内に関わらず75文字オーバーのエラーが出る不具合の修正<br>
 ver0.8 : 75文字制限突破(max:1024)の実装 ※184投下時不可,自己責任<br>
 ver0.9 : 先頭行と最終行の文字数カウント機能の追加(※末尾の< br >はカウントされません)<br>
 ver0.91 :　12/16から入力の仕様が変化し、コメントの反映が行えていなかった問題を解消  
 ver0.94 :  投コメのエディタのjsonを1コメント1行形式に置換して出力する機能を実装<br>
 ver0.95 :　画像読み込み機能を追加
 ver0.96 :　読み込んだ画像から色情報を取得・表示する機能を追加    

<br>
<br>
