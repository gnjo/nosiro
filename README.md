# nosiro
```
GOZ:I
名称はゴズ。時間制約シューティング。

ゴズの世界。ドローンが大量に発生している為、複製に制約がかかっている。
人類はワイアード世界で、また部品を組み立てる生活に逆行した。
人類は再度のアイデンティティを取得する。

装：コスト、基礎威力、チャージ容量、耐性、速度、慣性
鞭：コスト、威力、射程、ディレイ
銃：コスト、威力、弾数、装填時間
核：コスト、必要量、機能、パッシブかアクティブか
核はコストが許す限り幾つでも。道中で拾えばコストはかからない。

あらゆる機能は、全てアイテムとしてドロップする。
アイテムはデータフラグ制、一度取得すれば永続的に得られる。
装甲は三種類を揃える事で、追加される。零式体、零式腕、零式脚。

A:銃
B:加速、押しっぱなしの間はチャージ消費１
Y:鞭
X:核発動、会話その他動作
LR:核切替

ダイブ時間＝持ち時間－装備コスト
シナリオを一つクリアする毎に２秒持ち時間が増える。

電脳頭「おいおい、ここのゴズを倒そうと思ったら、インスペクターが必要だ。今日は見学なのか」
「ここの構造体に侵入するには、彼らと同じ機体が必要だ。ヤシロで調達できるんじゃないか」
「ダイブ時間とは複製抑止時間だ。敵がお前と同じスペックだったら、勝率は五分だろうがよ」
　安全率の観点から良くない。
　詰め込まされた箱庭とはアノニマスシティだ。

コストは、ダイブ時間に換算される。
装備にはランクがあり、ランクによってコストは大凡決まっている。
ランク１は、０～１秒。ランク２は１～２秒。ランクは最大コストを示す。
戦場は構造体という。ひとつの構造体は深度で示される。
対象深度が示され、達成する任務が多い。

リリーレイ「私達はリリーレイ。第二知性体。人類の安楽死を願う存在です」
シャイアー「人類同士で争っている場合ではないが、闘争とは力だ」
コバルト「そう、忘れたわ」
生足の赤い女「報酬がデータチップだなんて、余り物を押し付ける気じゃないでしょうね」
ガリコ「みんなあの女がいつ死ぬか賭けてるんですよ」
マシュマロと渾名される男「うむ、よし賭けてみよう。死んでも恨むなよ」
チョモランマ「やはりサンジェルマン」
ジンク「オーケーだ」

施設
クイーン：傭兵斡旋所。中央には無数のチューブが頭に接続された電脳頭が居る。
パンプス：アンセムの機体改造専門。対抗としてヤシロがある。
整備ドック：パンプスやヤシロの裏には大きなドックがある。
```

```
5sec rule

ダイブ時間は最も重要な資源である。
取得したコアは記録されドックで組み込む事ができる。
３＊３＊３シナリオあり、１つのシナリオをクリアするとエンディング。
ひとつのステージは進行度で表され、シナリオの進行度と同期する。
アイテム類はフラグ管理され、一度取得すれば永続的に使える。
小シナリオをクリアする毎に、ダイブ時間は永続的に２秒加算される。

ひとつのステージは隔壁で区切られている。
ひとつのステージは隔壁戦とゴズ戦に分けられている。
隔壁戦は大量のドローンが出現する。一定数倒すと隔壁が開く。ダイブ時間は常に減る。
ゴズ戦は強敵が出現する。ダイブ時間は止まるが、被弾するとダイブ時間が大きく減る。

３隔壁毎に、ゴズが待ち構えている。ゴズとはスキルフルの事。
ゴズを倒すと５秒追加される。
ゴズを無傷で倒すと５秒追加される。
ゴズへの弱点累計ダメージが５割以上で倒すと、５秒追加される。

コアを発動すると、倒した敵の数だけダイブ時間が延長する。


ダイブ時間＝持ち時間－装備コスト
持ち時間が許す限り装備を搭載できるが、ダイブ時間は減る。

クロガネ「ダイブ時間０秒で何をするんだ」

難易度は初期の持ち時間のみ。
S'tair：初期持ち時間３０秒
T'ender：初期持ち時間１５秒
U'ltima：初期持ち時間５秒

R'edMountain
G'reenLake
B'lueSky

P'urpleHaze
O'rangeNail
W'hiteRobe

L'unarian
E'arBigger
M'etropolitan

F'iveSeconds
A'irBooster
Q'ueen

シナリオは全てスタック式。

:S-R1G1B1-D010I09C05-X0X0X0...           00:00:00:
+------------------------------------------------+
|*Queen      | skill list                        |
| Build      |                                   |
| Core       |                                   |
| Data       |                                [Y]|
|!#Green1    +-----------------------------------+
| #Green2    | 010 Green1                        |
| #Red1      |                                   |
| #Red2      |         view back                 |
| #Red3      |                                   |
|        [+A]|                               [LR]|
+------------+-----------------------------------+
: NAV: Update #Green2 and #Red2                  :
:                                             [X]:
 
! is notice 
code:[mode]-[scenario]-[spec]-[equip]-[itemflgs] //all save data

ドローンから被弾すると、耐性があれば0.1s減少、耐性がなければ0.2s減少する。
ゴズの場合は、５倍。耐性があれば0.5s減少、耐性がなければ1.0s減少する。

```


```
5sec
```
```
1item/5sec
大方針 120秒で24個のアイテムをドロップする。
一つのステージは120秒以内。
強くなればなるほど、奥へ進める。

最も重要な要素、移動速度、ダイブ時間。
ステージは隔壁で区切られている。
１０体程度倒すと隔壁が開く。
雑魚は基本、弱点属性で一撃で倒す事ができる。

３の倍数毎にボスが居る。
１：
２：
３：ボス部屋


```
game idea
```
アイテムを拾いながら敵を倒していく。
シューティングゲームに近い。
敵を倒すと速度加速、生命力回復、魔石、永続強化を拾う事ができる。
速度加速アイテムはスタックされ、被弾する毎に一減る。
魔石はスタックされ、敵を倒すとゲージが貯まる、複数所持できる。
獲得した魔石は登録され、出撃時に一つだけ装備できる。
魔石４以上は、速度加速＋２に変わる。
敵を倒した際に、永続アイテムが手に入る事で自身を強化する。
強化項目は二つ、弾倉、生命力、払い飛距離。また銀貨を使用して同等の事ができる。
生命力と同じだけ加速できる。
道中、武器を取得できる。武器には強化限界が設定されている。３～２０。
防具は無いが、ウィップとガンと本体を強化する事で、マップを踏破する。

A：ウィップ
B：ダッシュ
Y：ガン
X：会話、イベント等
LRで魔石切替、魔石は自動発動

ウィップの系統。
スラッシュウィップ：最もオーソドックス。前方に払う。
パイルウィップ：三本の硬化した鞭を前に出す。
ロールウィップ：一回転し、最後に前方に払う。

ガンの系統。
レーザーガン：前方に太いレーザーを出す。
アサルトガン：最もオーソドックス。数を撃つ。
ショットガン：近距離で最も威力が高い。

ウィップとガンのダメージに違いは無いが、炎氷雷の属性武器がある。

魔石は比較的頻繁に発動する。ゲージは５。
敵を倒す：２
敵を連続で倒すと追加１。
ウィップ当てる：１
ガンを当てる：１
ウィップの次にガンを当てると追加１。
```
```
メイン画面
シナリオがさみだれでスタックされ、次々に進める。

＊エントリ：基本はエントリ、エントリ、エントリ。
　リトライ：クリア済みをもう一度行える。
　ドック：装備と強化。
　記録：セーブ等。

おいおい、パイルウィップで壊す隔壁があるって云ったじゃないか。
ないなら、まず探してこいよ。

そんな装備で大丈夫か。
ウィップ＋５以上じゃなければこの辺りの敵に通用しないぜ。

貴方の目となる。チョモランマだ。
オーケー、チョモランマ。こちらラビットだ。兎じゃない、ロボットの訛りだ。

```



