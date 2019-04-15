---
title: "相手インク影響軽減"
description: "スプラトゥーン2 相手インク影響軽減"
keywords: ["splatoon2", "スプラトゥーン2", "ギアパワー", "ギア", "効果", "グラフ", "相手インク影響軽減", "安全靴"]
date: 2019-01-10T00:41:14+09:00
draft: flase
---

相手インク影響軽減は相手インク上での各種マイナス効果を軽減します。軽減対象が全てで4種類あります。

* 移動速度
* 最大ダメージ量
* 1フレーム辺りのダメージ量
* 無敵フレーム

これらのうち移動速度は ver4.6.0 でさらに効果が出やすくなったが今の所 ver4.5.0 しか検証していません。検証したら直します。

#### 移動速度

DU/s で最大 0.84 となります。相手のインクの影響なしヒト速 GP0 での重量ブキで 0.88 DU/s なのでそれに近い動きになる。

まったく付けていない時は 0.24 DU/s これに最大で 0.6 DU/s 加算され 0.84 DU/s となる。ver 4.6.0 で強化され [相手インク影響軽減 ver4.6.0 の変更検証](https://ika.ninja/memo/aite_ink_ver_4_6_0) をした結果からの数値で誤差がある可能性もあります。

グラフは以下の通り

<iframe width="800" height="450" src="https://datastudio.google.com/embed/reporting/1QPAzR5saDn8Dd8O-tHWOenJz_P0Avbzg/page/mhTm" frameborder="0" style="border:0" allowfullscreen></iframe>

#### 最大ダメージ量

1フレーム辺りのダメージの累積最大ダメージ値となります。何も付けていなければ最大40ダメージ。限界まで付けた場合 20ダメージまでしか受けなくなります。

この効果を軸に考えた時は例えば GP12 まで付けた場合 32.86 ダメージが最大値となり、疑似確定3の33.3ダメージのブキ相手に遭遇した時に相手インクにいくら乗っていても 2確状態が生まれないという利点があります。

グラフは以下の通り

<iframe width="800" height="450" src="https://datastudio.google.com/embed/reporting/1QPAzR5saDn8Dd8O-tHWOenJz_P0Avbzg/page/XhTm" frameborder="0" style="border:0" allowfullscreen></iframe>

#### 1フレーム辺りのダメージ量

1フレームあたりのダメージ量について何もついてない状態で 0.3 、GP26以上で 0.1 となりそれ以上は少なくなりません。

また小数点以下第二位は切り捨てられており以下の表のような範囲でダメージ量が変わります。

|GP|ダメージ量|
|---|---|
|0|0.3|
|3以上, 24以下|0.2|
|26以上|0.1|

この3つのバリエーションしか無いために基本的にはこの効果を軸につけるばあいは GP3、あるいはGP26、のどちらかを選択することになります。

基本的に1フレームあたりのダメージが 0.3 から 0.2 になるアドバンテージは1秒間に相手インク上でうけるダメージが18から12へ6減るという大きなアドバンテージになるので最低でも 3GP つけると良いと思われる。

GP 26以上になると秒間ダメージがたったの6となるが疑似確定相手とかに対するアドバンテージはここでは得られない(次の無敵フレームが影響でるかと思われる)

<iframe width="800" height="450" src="https://datastudio.google.com/embed/reporting/1QPAzR5saDn8Dd8O-tHWOenJz_P0Avbzg/page/pgTm" frameborder="0" style="border:0" allowfullscreen></iframe>

#### 無敵フレーム

無敵フレームは相手のインク上でのダメージが0になるフレーム数です。最大で 39フレーム となり 0.65 秒 あるいは スプラシューターを 6.5 発打っている間無敵です。

何も付けてなければ 0 フレームで即座に毎フレームごと 0.3 のダメージを受けます。GP3 で10フレーム程度になり1フレーム辺り 0.2 ダメージしか受けなくなるためにかなりのアドバンテージを得られるかと思います。

<iframe width="800" height="450" src="https://datastudio.google.com/embed/reporting/1QPAzR5saDn8Dd8O-tHWOenJz_P0Avbzg/page/LiTm" frameborder="0" style="border:0" allowfullscreen></iframe>
