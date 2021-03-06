+++
title = "ギアパワー"
weight = 10
alwaysopen = true
description = "スプラトゥーン2 ギアパワーの効果などまとめ"
keywords = ["splatoon2", "スプラトゥーン2", "ギアパワー", "ギア", "効果", "グラフ", "メインインク効率アップ", "イカ速", "ヒト速", "安全靴", "スパ短", "復活時間短縮", "スペ増", "スペ減"]
+++

- [インク効率アップ(メイン)](https://ika.ninja/gear/1_main_ink/)
- [インク効率アップ(サブ)](https://ika.ninja/gear/2_sub_ink/)
- [インク回復力アップ](https://ika.ninja/gear/3_rec_ink/)
- [イカダッシュ速度アップ](https://ika.ninja/gear/4_ika_speed/)
- [ヒト移動速度アップ](https://ika.ninja/gear/5_hito_speed/)
- [スペシャル増加アップ減少ダウン](https://ika.ninja/gear/6_special_up_down/)
- [スーパージャンプ時間短縮](https://ika.ninja/gear/7_super_jump/)
- [復活時間短縮](https://ika.ninja/gear/8_revi_time/)
- [相手インク影響軽減](https://ika.ninja/gear/9_aite_ink/)

## ギアパワー関連情報

ギアパワーのかかり方などについてまとめ

この検証データ類は個人的な検証とか予想で恐らくの値を出しています。間違っていても許して欲しい。

以下基礎知識について

### メインギア、サブギアとその数値表現

基本的にギアはメインギアパワー(付け替え不可能)を1つ、サブギアパワー(付け替え可能)を3つで1つのギアとなる。

このサイト内ではメインギアパワーを10とし、サブギアパワーを3とし、1つのギアで最大19、単位はGPを使う。

例えば

* メインギア:メイン性能アップ
* サブギア1:イカ速
* サブギア2:イカ速
* サブギア3:スーパージャンプ短縮

といったギアがあった時

* メイン性能アップ 10GP
* イカ速度 6GP
* スーパージャンプ短縮 3GP

といった表記になる。この表現はギアパワー計算機などのツールなども使っている。

すべて同じギアパワーに揃えた場合は57GPということになる。

### ギアパワーのかかり方について

#### 効果量

ギアパワーのかかり方は段階的に効果が出てきます。(イカニンジャなど特殊な例は除きます)

基本的にギアパワーの乗り方は少ない数値であれば効果が出やすく、最大効果量に近づけば近づくほどGPに対しての効果量が減っていきます。

ガンマ補正がされる例と特殊なガンマ補正のガンマ補正(スプラマニューバーのメイン性能アップのみそのような補正)とかがあります。

補正はどちらかというと上方補正、少ないギアパワーでの効果量が上がるという意図のものが多くスプラシューターではジャンプ時ブレ補正がGP10時に50％軽減される等があります。

#### 効果量限界

一部というかメイン性能アップのダメージ量増加に限り効果量の限界があり要するに疑似2確、疑似3確定のこと

これは単純にダメージ量増加に伴い確定数が変化するあたりで強制的に効果打ち切りとなる。

#### その他特殊例

相手インク軽減において敵インク上でのスリップダメージについては何故か段階的に効果キャップがある。

スリップダメージ以外は他とあまり変わりないので意図している？
あるいは浮動少数計算の誤差を避けるための開発側のライブラリ依存とかが予想できなくもない。

#### 各効果の詳細は左メニューより
