# Shadowverse-wb-json

[カードリスト](https://shadowverse-wb.com/ja/deck/cardslist)を基に作成しています

公式サイト　カードリストの部分について
https://shadowverse-wb.com/web/CardList/cardList?offset=0の後ろに

&class={0~7}
```
0   ->  ニュートラル
1   ->  エルフ
2   ->  ロイヤル
3   ->  ウィッチ
4   ->  ドラゴン
5   ->  ナイトメア
6   ->  ビショップ
7   ->  ネメシス
```
&class=コスト値

## 構造

```json
    "card_details": {
      "10001110": {
        "common": {
          "card_id": 10001110,
          "name": "不屈のファイター",
          "name_ruby": "\u003Cruby class=\"card-main-title-ruby\" name-ruby=\"ふくつ\"\u003E不屈\u003Crt\u003Eふくつ\u003C/rt\u003E\u003C/ruby\u003Eのファイター",
          "base_card_id": 10001110,
          "card_resource_id": 100011100,
          "atk": 2,
          "life": 2,
          "flavour_text": "争いだらけの世界で、頼れるものは自分の力だけだ。\n勝利も伝説も、全て俺だけが手にしてやろう。",
          "skill_text": "【\u003Ccolor=Keyword\u003Eエンハンス\u003C/color\u003E_4】これは+3/+3する。",
          "card_set_id": 10000,
          "type": 1,
          "class": 0,
          "tribes": [0],
          "cost": 2,
          "rarity": 1,
          "cv": "松岡禎丞",
          "illustrator": "tricky胡坐",
          "questions": [],
          "is_token": false,
          "is_include_rotation": true,
          "card_image_hash": "63937d009aa549baac4885413090ed27",
          "card_banner_image_hash": "995d149dec134d749793bfde1fed4473"
        },
        "evo": {
          "card_resource_id": 100011101,
          "flavour_text": "争いのない世界こそ、俺の切り開きたかった未来だ。\n頼るのは自分だけ。敵も憎しみも、全て俺が引き受ける。",
          "skill_text": "【\u003Ccolor=Keyword\u003Eエンハンス\u003C/color\u003E_4】これは+3/+3する。",
          "card_image_hash": "8f1ab12418fc4d0aa41f96eff6211593",
          "card_banner_image_hash": "8417135a9a8f4b3ab9ec136c937b4e80"
        },
        "style_card_list": []
      },
    }
```

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
token           ->  トークン(カードから生成されるカード※デッキには入れれない)
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