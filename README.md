# Shadowverse-wb-json

[カードリスト](https://shadowverse-wb.com/ja/deck/cardslist)を基に作成しています

## json 構造

```
name            ->  カード名
id              ->  カードID
pp              ->  コストPP
craft           ->  クラス※1
rarity          ->  レアリティ
type            ->  分類※2
trait           ->  タイプ※3
expansion       ->  排出パック
baseFlair       ->  通常フレーバーテキスト
baseAtk         ->  攻撃力
baseDef         ->  体力
baseEffect      ->  通常時効果
evoFlair        ->  進化フレーバーテキスト
evoAtk          ->  攻撃力(進化)
evoDef          ->  体力(進化)
evoEffect       ->  進化時効果
sevoAtk         ->  攻撃力(超進化)
sevoDef         ->  体力(超進化)
sevoEffect      ->  超進化時効果
crest           ->  クレスト効果
cv              ->  cv
illustrator     ->  イラストレーター
card_image      ->  通常カード
evo_card_image  ->  進化後カード
```
### ※1 クラス

```
ニュートラル
エルフ
ロイヤル
ウィッチ
ドラゴン
ナイトメア
ビショップ
ネメシス
```

### ※2 分類

```
フォロワー
スペル
アミュレット
```

### ※3 タイプ

```
-
兵士
ルミナス
レヴィオン
妖精
死者
土の印
マナリア
ゴーレム
式神
アーティファクト
人形
海洋
アナテマ
```