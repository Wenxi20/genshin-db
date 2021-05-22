# Examples

First start off with:
```js
const genshindb = require('genshin-db');
```

## Table of Contents

- [genshindb.characters(query[, opts])](#genshindbcharactersquery-opts)
- [genshindb.talents(query[, opts])](#genshindbtalentsquery-opts)
- [genshindb.constellations(query[, opts])](#genshindbconstellationsquery-opts)
- [genshindb.weapons(query[, opts])](#genshindbweaponsquery-opts)
- [genshindb.weaponmaterialtypes(query[, opts])](#genshindbweaponmaterialtypesquery-opts)
- [genshindb.talentmaterialtypes(query[, opts])](#genshindbtalentmaterialtypesquery-opts)
- [genshindb.artifacts(query[, opts])](#genshindbartifactsquery-opts)
- [genshindb.foods(query[, opts])](#genshindbfoodsquery-opts)
- [genshindb.elements(query[, opts])](#genshindbelementsquery-opts)
- [genshindb.rarity(query[, opts])](#genshindbrarityquery-opts)

## genshindb.characters(query[, opts])]

<details>
<summary>genshindb.characters('<b>names', { matchCategories: true }</b>)</summary>

```js
[
  'Aether',   'Albedo',    'Amber',
  'Barbara',  'Beidou',    'Bennett',
  'Chongyun', 'Diluc',     'Diona',
  'Eula',     'Fischl',    'Ganyu',
  'Hu Tao',   'Jean',      'Kaeya',
  'Keqing',   'Klee',      'Lisa',
  'Lumine',   'Mona',      'Ningguang',
  'Noelle',   'Qiqi',      'Razor',
  'Rosaria',  'Sucrose',   'Tartaglia',
  'Venti',    'Xiangling', 'Xiao',
  'Xingqiu',  'Xinyan',    'Yanfei',
  'Zhongli'
]
```

</details>
<details>
<summary>genshindb.characters('<b>ganyu'</b>)</summary>

```js
{
  name: 'Ganyu',
  title: 'Plenilune Gaze',
  description: 'The secretary at Yuehai Pavilion. The blood of the qilin, an illuminated beast, flows within her veins.',
  rarity: '5',
  element: 'Cryo',
  weapontype: 'Bow',
  substat: 'CRIT DMG',
  gender: 'Female',
  body: 'GIRL',
  association: 'LIYUE',
  region: 'Liyue',
  affiliation: 'Yuehai Pavilion',
  birthdaymmdd: '12/2',
  birthday: 'December 2',
  constellation: 'Sinae Unicornis',
  cv: {
    english: 'Jennifer Losi',
    chinese: '林簌',
    japanese: '上田麗奈',
    korean: '김선혜'
  },
  talentmaterialtype: 'Diligence',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/0/0a/Character_Ganyu_Thumb.png',
    card: 'https://static.wikia.nocookie.net/gensin-impact/images/8/8d/Character_Ganyu_Card.png',
    portrait: 'https://static.wikia.nocookie.net/gensin-impact/images/a/a0/Character_Ganyu_Portrait.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_icon/UI_AvatarIcon_Ganyu.png',
    sideicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_side_icon/UI_AvatarIcon_Side_Ganyu.png',
    cover1: 'https://uploadstatic-sea.mihoyo.com/contentweb/20210105/2021010519275372324.png',
    cover2: 'https://uploadstatic-sea.mihoyo.com/contentweb/20210105/2021010519280045054.png',
    'hoyolab-avatar': 'https://img-os-static.hoyolab.com/communityWeb/upload/4af4adf192a35db2dd76d9718acc7bc8.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Ganyu' },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.characters('<b>amber', { resultLanguage: 'JP' }</b>)</summary>

```js
{
  name: 'アンバー',
  title: '飛行チャンピオン',
  description: '元気満々な女の子、騎士団で最も優秀で、最後の偵察騎士である。',
  rarity: '4',
  element: '炎',
  weapontype: '弓',
  substat: '攻撃力',
  gender: '女',
  body: 'GIRL',
  association: 'MONDSTADT',
  region: 'Mondstadt',
  affiliation: '西風騎士団',
  birthdaymmdd: '8/10',
  birthday: '8月10日',
  constellation: '小兎座',
  cv: {
    english: 'Kelly Baskin',
    chinese: '蔡书瑾',
    japanese: '石見舞菜香',
    korean: '김연우'
  },
  talentmaterialtype: '',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/c/c6/Character_Amber_Thumb.png',
    card: 'https://static.wikia.nocookie.net/gensin-impact/images/2/26/Character_Amber_Card.jpg',
    portrait: 'https://static.wikia.nocookie.net/gensin-impact/images/0/00/Character_Amber_Portrait.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_icon/UI_AvatarIcon_Ambor.png',
    sideicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_side_icon/UI_AvatarIcon_Side_Ambor.png',
    cover1: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191009/2019100914372396510.png',
    cover2: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191009/2019100914390892929.png',
    'hoyolab-avatar': 'https://img-os-static.hoyolab.com/avatar/avatar40019.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Amber' },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.characters('<b>アンバー', { queryLanguages: 'Japanese', resultLanguage: 'Spanish' }</b>)</summary>

```js
{
  name: 'Amber',
  title: 'la Campeona de Vuelo',
  description: 'Siempre enérgica y llena de vida, Amber es la mejor exploradora de los Caballeros de Favonius, aunque también es la única...',
  rarity: '4',
  element: 'Pyro',
  weapontype: 'Arco',
  substat: 'ATQ',
  gender: 'Femenino',
  body: 'GIRL',
  association: 'MONDSTADT',
  region: 'Mondstadt',
  affiliation: 'Caballeros de Favonius',
  birthdaymmdd: '8/10',
  birthday: '10 de agosto',
  constellation: 'Lepus Minor',
  cv: {
    english: 'Kelly Baskin',
    chinese: '蔡书瑾',
    japanese: '石見舞菜香',
    korean: '김연우'
  },
  talentmaterialtype: 'Libertad',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/c/c6/Character_Amber_Thumb.png',
    card: 'https://static.wikia.nocookie.net/gensin-impact/images/2/26/Character_Amber_Card.jpg',
    portrait: 'https://static.wikia.nocookie.net/gensin-impact/images/0/00/Character_Amber_Portrait.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_icon/UI_AvatarIcon_Ambor.png',
    sideicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_side_icon/UI_AvatarIcon_Side_Ambor.png',
    cover1: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191009/2019100914372396510.png',
    cover2: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191009/2019100914390892929.png',
    'hoyolab-avatar': 'https://img-os-static.hoyolab.com/avatar/avatar40019.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Amber' },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.characters('<b>childe', { matchAliases: true }</b>)</summary>

```js
{
  name: 'Tartaglia',
  title: 'Childe',
  description: 'No. 11 of The Harbingers, also known as "Childe." His name is highly feared on the battlefield.',
  rarity: '5',
  element: 'Hydro',
  weapontype: 'Bow',
  substat: 'Hydro DMG Bonus',
  gender: 'Male',
  body: 'MALE',
  association: 'FATUI',
  region: 'Snezhnaya',
  affiliation: 'Fatui',
  birthdaymmdd: '7/20',
  birthday: 'July 20',
  constellation: 'Monoceros Caeli',
  cv: {
    english: 'Griffin Burns',
    chinese: '鱼冻',
    japanese: '木村良平',
    korean: '남도형'
  },
  talentmaterialtype: 'Freedom',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/5/53/Character_Tartaglia_Thumb.png',
    card: 'https://static.wikia.nocookie.net/gensin-impact/images/4/4c/Character_Tartaglia_Card.png',
    portrait: 'https://static.wikia.nocookie.net/gensin-impact/images/3/3a/Character_Tartaglia_Portrait.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_icon/UI_AvatarIcon_Tartaglia.png',
    sideicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_side_icon/UI_AvatarIcon_Side_Tartaglia.png',
    cover1: 'https://uploadstatic-sea.mihoyo.com/contentweb/20201103/2020110321160453386.png',
    cover2: 'https://uploadstatic-sea.mihoyo.com/contentweb/20201103/2020110321234137061.png',
    'hoyolab-avatar': 'https://img-os-static.hoyolab.com/communityWeb/upload/34ebaeb164a8b447dbe52afaae3e1f63.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Tartaglia' },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.characters('<b>carmen', { matchAliases: true }</b>)</summary>

```js
{
  name: 'Venti',
  title: 'Windborne Bard',
  description: "One of the many bards of Mondstadt, who freely wanders the city's streets and alleys.",
  rarity: '5',
  element: 'Anemo',
  weapontype: 'Bow',
  substat: 'Energy Recharge',
  gender: 'Male',
  body: 'BOY',
  association: 'MONDSTADT',
  region: 'Mondstadt',
  affiliation: 'Mondstadt',
  birthdaymmdd: '6/16',
  birthday: 'June 16',
  constellation: 'Carmen Dei',
  cv: {
    english: 'Erika Harlacher',
    chinese: '喵酱',
    japanese: '村瀬歩',
    korean: '정유정'
  },
  talentmaterialtype: 'Ballad',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/8/8d/Character_Venti_Thumb.png',
    card: 'https://static.wikia.nocookie.net/gensin-impact/images/7/76/Character_Venti_Card.jpg',
    portrait: 'https://static.wikia.nocookie.net/gensin-impact/images/c/cf/Character_Venti_Portrait.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_icon/UI_AvatarIcon_Venti.png',
    sideicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/character_side_icon/UI_AvatarIcon_Side_Venti.png',
    cover1: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191122/2019112210305833310.png',
    cover2: 'https://uploadstatic-sea.mihoyo.com/contentweb/20191122/2019112211143037621.png',
    'hoyolab-avatar': 'https://img-os-static.hoyolab.com/avatar/avatar40022.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Venti' },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.characters('<b>december', { matchCategories: true }</b>)</summary>

```js
[ 'Ganyu', 'Zhongli' ]
```

</details>
<details>
<summary>genshindb.characters('<b>pyro', { matchCategories: true }</b>)</summary>

```js
[
  'Amber',  'Bennett',
  'Diluc',  'Hu Tao',
  'Klee',   'Xiangling',
  'Xinyan', 'Yanfei'
]
```

</details>
<details>
<summary>genshindb.characters('<b>geo dmg', { matchCategories: true }</b>)</summary>

```js
[ 'Albedo', 'Ningguang', 'Zhongli' ]
```

</details>
<details>
<summary>genshindb.characters('<b>liyue', { matchCategories: true }</b>)</summary>

```js
[
  'Beidou',  'Chongyun',
  'Ganyu',   'Hu Tao',
  'Keqing',  'Ningguang',
  'Qiqi',    'Xiangling',
  'Xiao',    'Xingqiu',
  'Xinyan',  'Yanfei',
  'Zhongli'
]
```

</details>
<details>
<summary>genshindb.characters('<b>sword', { matchCategories: true }</b>)</summary>

```js
[
  'Aether',  'Albedo',
  'Bennett', 'Jean',
  'Kaeya',   'Keqing',
  'Lumine',  'Qiqi',
  'Xingqiu'
]
```

</details>
<details>
<summary>genshindb.characters('<b>ballad', { matchCategories: true }</b>)</summary>

```js
[ 'Albedo', 'Fischl', 'Kaeya', 'Lisa', 'Rosaria', 'Venti' ]
```

</details>
<details>
<summary>genshindb.characters('<b>klee'</b>)<b>.stats(90)</b></summary>

```js
{
  level: 90,
  ascension: 6,
  hp: 10286.565419930499,
  attack: 310.93189668962077,
  defense: 614.8434950278315,
  specialized: 0.2879999876022339
}
```

</details>
<details>
<summary>genshindb.characters('<b>klee'</b>)<b>.stats(80)</b></summary>

```js
{
  level: 80,
  ascension: 5,
  hp: 9075.60273520241,
  attack: 274.32835675104525,
  defense: 542.4622838181458,
  specialized: 0.2160000056028366
}
```

</details>
<details>
<summary>genshindb.characters('<b>klee'</b>)<b>.stats(80, '+')</b></summary>

```js
{
  level: 80,
  ascension: 6,
  hp: 9563.45283285866,
  attack: 289.0738706670609,
  defense: 571.6222874802552,
  specialized: 0.2879999876022339
}
```

</details>
<details>
<summary>genshindb.characters('<b>aether'</b>)<b>.stats(12)</b></summary>

```js
{
  level: 12,
  ascension: 0,
  hp: 1739.6972508560866,
  attack: 33.97766494134521,
  defense: 109.18529665203096,
  specialized: 0
}
```

</details>

## genshindb.talents(query[, opts])]

<details>
<summary>genshindb.talents('<b>names', { matchCategories: true }</b>)</summary>

```js
[
  'Albedo',         'Amber',
  'Barbara',        'Beidou',
  'Bennett',        'Chongyun',
  'Diluc',          'Diona',
  'Eula',           'Fischl',
  'Ganyu',          'Hu Tao',
  'Jean',           'Kaeya',
  'Keqing',         'Klee',
  'Lisa',           'Mona',
  'Ningguang',      'Noelle',
  'Qiqi',           'Razor',
  'Rosaria',        'Sucrose',
  'Tartaglia',      'Traveler (Anemo)',
  'Traveler (Geo)', 'Venti',
  'Xiangling',      'Xiao',
  'Xingqiu',        'Xinyan',
  'Yanfei',         'Zhongli'
]
```

</details>
<details>
<summary>genshindb.talents('<b>ninguang'</b>)</summary>

```js
{
  name: 'Ningguang',
  combat1: {
    name: 'Normal Attack: Sparkling Scatter',
    info: '**Normal Attack**\n' +
      'Shoots gems that deal Geo DMG.\n' +
      'Upon hit, this grants Ningguang 1 Star Jade.\n' +
      '\n' +
      '**Charged Attack**\n' +
      'Consumes a certain amount of stamina to fire off a giant gem that deals Geo DMG.\n' +
      'If Ningguang has any Star Jades, unleashing a Charged Attack will cause the Star Jades to be fired at the enemy as well, dealing additional DMG.\n' +
      '\n' +
      '**Plunging Attack**\n' +
      'Gathering the might of Geo, Ningguang plunges towards the ground from mid-air, damaging all opponents in her path. Deals AoE Geo DMG upon impact with the ground.',
    attributes: {
      labels: [
        'Normal Attack DMG|{param1:F1P}',
        'Charged Attack DMG|{param2:P}',
        'DMG per Star Jade|{param3:F1P}',
        'Charged Attack Stamina Cost|{param4:F1}',
        'Plunge DMG|{param5:F1P}',
        'Low/High Plunge DMG|{param6:P}/{param7:P}'
      ],
      parameters: {
        param1: [
          0.2800000011920929,
          0.3009999990463257,
          0.32199999690055847,
          0.3499999940395355,
          0.3709999918937683,
          0.3919999897480011,
          0.41999998688697815,
          0.4480000138282776,
          0.47600001096725464,
          0.5040000081062317,
          0.5331199765205383,
          0.5712000131607056,
          0.609279990196228,
          0.6473600268363953,
          0.6854400038719177
        ],
        param2: [
          1.7408000230789185,  1.871359944343567,
           2.001919984817505, 2.1760001182556152,
          2.3065600395202637,  2.437119960784912,
          2.6112000942230225, 2.7852799892425537,
           2.959359884262085, 3.1334400177001953,
          3.3144829273223877,  3.551232099533081,
          3.7879810333251953,  4.024730205535889,
           4.261477947235107
        ],
        param3: [
          0.4959999918937683, 0.5332000255584717,
          0.5703999996185303, 0.6200000047683716,
          0.6571999788284302, 0.6944000124931335,
          0.7440000176429749, 0.7936000227928162,
          0.8432000279426575,  0.892799973487854,
           0.944383978843689, 1.0118399858474731,
          1.0792959928512573, 1.1467519998550415,
          1.2142080068588257
        ],
        param4: [
          50, 50, 50, 50, 50, 50,
          50, 50, 50, 50, 50, 50,
          50, 50, 50
        ],
        param5: [
          0.5682880282402039, 0.6145439743995667,
          0.6607999801635742, 0.7268800139427185,
          0.7731360197067261, 0.8259999752044678,
           0.898688018321991, 0.9713760018348694,
          1.0440640449523926,   1.12336003780365,
          1.2026560306549072, 1.2819520235061646,
          1.3612480163574219, 1.4405440092086792,
          1.5198400020599365
        ],
        param6: [
           1.136335015296936,  1.228827953338623,
          1.3213200569152832, 1.4534519910812378,
          1.5459439754486084, 1.6516499519348145,
          1.7969950437545776, 1.9423400163650513,
           2.087686061859131,  2.246243953704834,
           2.404802083969116, 2.5633609294891357,
           2.721919059753418, 2.8804779052734375,
          3.0390360355377197
        ],
        param7: [
          1.4193439483642578,  1.534872055053711,
          1.6504000425338745,  1.815440058708191,
          1.9309680461883545,  2.062999963760376,
            2.24454402923584, 2.4260880947113037,
          2.6076319217681885,    2.8056800365448,
           3.003727912902832, 3.2017760276794434,
          3.3998239040374756,  3.597872018814087,
           3.795919895172119
        ]
      }
    }
  },
  combat2: {
    name: 'Jade Screen',
    info: 'Ningguang creates a Jade Screen out of gold, obsidian and her great opulence, dealing AoE Geo DMG.\n' +
      '\n' +
      '**Jade Screen**\n' +
      "·Blocks opponents' projectiles.\n" +
      "·Endurance scales based on Ningguang's Max HP.\n" +
      '\n' +
      'Jade Screen is considered a Geo Construct and can be used to block certain attacks, but cannot be climbed. Only one Jade Screen may exist at any one time.',
    description: 'The canvas of stars is written upon this jade screen.',
    attributes: {
      labels: [
        'Inherited HP|{param3:F1P}',
        'Skill DMG|{param2:P}',
        'CD|{param4:F1}s'
      ],
      parameters: {
        param1: [
          -0.49900001287460327,
          -0.4690000116825104,
          -0.4390000104904175,
          -0.4000000059604645,
          -0.3700000047683716,
          -0.3400000035762787,
          -0.3009999990463257,
          -0.2619999945163727,
          -0.22300000488758087,
          -0.18400000035762787,
          -0.14499999582767487,
          -0.10599999874830246,
          -0.06700000166893005,
          -0.02800000086426735,
          0.010999999940395355
        ],
        param2: [
           2.303999900817871,  2.476799964904785,
           2.649600028991699,  2.880000114440918,
           3.052799940109253,  3.225600004196167,
          3.4560000896453857, 3.6863999366760254,
           3.916800022125244,  4.147200107574463,
           4.377600193023682,  4.607999801635742,
           4.895999908447266,  5.184000015258789,
          5.4720001220703125
        ],
        param3: [
          0.5009999871253967,  0.531000018119812,
          0.5609999895095825, 0.6000000238418579,
          0.6299999952316284, 0.6600000262260437,
          0.6990000009536743, 0.7379999756813049,
          0.7770000100135803, 0.8159999847412109,
          0.8550000190734863, 0.8939999938011169,
          0.9330000281333923,  0.972000002861023,
          1.0110000371932983
        ],
        param4: [
          12, 12, 12, 12, 12, 12,
          12, 12, 12, 12, 12, 12,
          12, 12, 12
        ]
      }
    }
  },
  combat3: {
    name: 'Starshatter',
    info: 'Gathering a great number of gems, Ningguang scatters them all at once, sending homing projectiles at her opponents that deal massive Geo DMG.\n' +
      'If Starshatter is cast when a Jade Screen is nearby, the Jade Screen will fire additional gem projectiles at the same time.',
    description: 'Stars shatter. Silence falls.',
    attributes: {
      labels: [
        'DMG Per Gem|{param1:F1P}',
        'CD|{param2:F1}s',
        'Energy Cost|{param3:I}'
      ],
      parameters: {
        param1: [
          0.8695999979972839,
          0.9348199963569641,
          1.000040054321289,
          1.0870000123977661,
          1.1522200107574463,
          1.2174400091171265,
          1.3043999671936035,
          1.3913600444793701,
          1.4783200025558472,
          1.5652799606323242,
          1.6522400379180908,
          1.7391999959945679,
          1.8479000329971313,
          1.9565999507904053,
          2.0652999877929688
        ],
        param2: [
          12, 12, 12, 12, 12, 12,
          12, 12, 12, 12, 12, 12,
          12, 12, 12
        ],
        param3: [
          40, 40, 40, 40, 40, 40,
          40, 40, 40, 40, 40, 40,
          40, 40, 40
        ]
      }
    }
  },
  passive1: {
    name: 'Backup Plan',
    info: 'When Ningguang is in possession of Star Jades, her Charged Attack does not consume Stamina.'
  },
  passive2: {
    name: 'Strategic Reserve',
    info: 'A character that passes through the **Jade Screen** will gain a 12% Geo DMG Bonus for 10s.'
  },
  passive3: {
    name: 'Trove of Marvelous Treasures',
    info: 'Displays the location of nearby **ore veins** (Iron Ore, White Iron Ore, Crystal Ore, Magical Crystal Ore, and Starsilver) on the mini-map.'
  },
  images: {
    combat1: '',
    combat2: '',
    combatsp: '',
    combat3: '',
    passive1: '',
    passive2: '',
    passive3: ''
  }
}
```

</details>
<details>
<summary>genshindb.talents('<b>klee'</b>)<b>.passive3</b></summary>

```js
{
  name: 'All Of My Treasures!',
  info: 'Displays the location of nearby **resources unique to Mondstadt** on the mini-map.'
}
```

</details>
<details>
<summary>genshindb.talents('<b>mona'</b>)<b>.combat1</b></summary>

```js
{
  name: 'Normal Attack: Ripple of Fate',
  info: '**Normal Attack**\n' +
    'Perform up to 4 water splash attacks that deal Hydro DMG.\n' +
    '\n' +
    '**Charged Attack**\n' +
    'Consumes a certain amount of Stamina to deal AoE Hydro DMG after a short casting time.\n' +
    '\n' +
    '**Plunging Attack**\n' +
    'Gathering the might of Hydro, Mona plunges towards the ground from mid-air, damaging all opponents in her path. Deals AoE Hydro DMG upon impact with the ground.',
  attributes: {
    labels: [
      '1-Hit DMG|{param1:F1P}',
      '2-Hit DMG|{param2:F1P}',
      '3-Hit DMG|{param3:F1P}',
      '4-Hit DMG|{param4:F1P}',
      'Charged Attack DMG|{param5:P}',
      'Charged Attack Stamina Cost|{param6:F1}',
      'Plunge DMG|{param7:F1P}',
      'Low/High Plunge DMG|{param8:P}/{param9:P}'
    ],
    parameters: {
      param1: [
        0.37599998712539673,
        0.4041999876499176,
        0.4323999881744385,
        0.4699999988079071,
        0.498199999332428,
        0.5264000296592712,
        0.5640000104904175,
        0.6015999913215637,
        0.63919997215271,
        0.676800012588501,
        0.7143999934196472,
        0.7519999742507935,
        0.7990000247955322,
        0.8460000157356262,
        0.8930000066757202
      ],
      param2: [
        0.36000001430511475,
        0.3869999945163727,
        0.414000004529953,
        0.44999998807907104,
        0.47699999809265137,
        0.5040000081062317,
        0.5400000214576721,
        0.5759999752044678,
        0.6119999885559082,
        0.6480000019073486,
        0.6840000152587891,
        0.7200000286102295,
        0.7649999856948853,
        0.8100000023841858,
        0.8550000190734863
      ],
      param3: [
        0.4480000138282776,
        0.48159998655319214,
        0.5152000188827515,
        0.5600000023841858,
        0.5935999751091003,
        0.6272000074386597,
        0.671999990940094,
        0.7167999744415283,
        0.7616000175476074,
        0.8064000010490417,
        0.8511999845504761,
        0.8960000276565552,
        0.9520000219345093,
        1.0080000162124634,
        1.0640000104904175
      ],
      param4: [
        0.5616000294685364, 0.6037200093269348,
        0.6458399891853333, 0.7020000219345093,
        0.7441200017929077, 0.7862399816513062,
        0.8424000144004822, 0.8985599875450134,
        0.9547200202941895, 1.0108799934387207,
         1.067039966583252, 1.1232000589370728,
        1.1934000253677368, 1.2635999917984009,
         1.333799958229065
      ],
      param5: [
        1.4972000122070312, 1.6094900369644165,
        1.7217799425125122,  1.871500015258789,
        1.9837900400161743, 2.0960800647735596,
         2.245800018310547,  2.395519971847534,
        2.5452399253845215,  2.694960117340088,
        2.8506689071655273,  3.054287910461426,
         3.257906913757324, 3.4615259170532227,
        3.6651461124420166
      ],
      param6: [
        50, 50, 50, 50, 50, 50,
        50, 50, 50, 50, 50, 50,
        50, 50, 50
      ],
      param7: [
        0.5682880282402039, 0.6145439743995667,
        0.6607999801635742, 0.7268800139427185,
        0.7731360197067261, 0.8259999752044678,
         0.898688018321991, 0.9713760018348694,
        1.0440640449523926,   1.12336003780365,
        1.2026560306549072, 1.2819520235061646,
        1.3612480163574219, 1.4405440092086792,
        1.5198400020599365
      ],
      param8: [
         1.136335015296936,  1.228827953338623,
        1.3213200569152832, 1.4534519910812378,
        1.5459439754486084, 1.6516499519348145,
        1.7969950437545776, 1.9423400163650513,
         2.087686061859131,  2.246243953704834,
         2.404802083969116, 2.5633609294891357,
         2.721919059753418, 2.8804779052734375,
        3.0390360355377197
      ],
      param9: [
        1.4193439483642578,  1.534872055053711,
        1.6504000425338745,  1.815440058708191,
        1.9309680461883545,  2.062999963760376,
          2.24454402923584, 2.4260880947113037,
        2.6076319217681885,    2.8056800365448,
         3.003727912902832, 3.2017760276794434,
        3.3998239040374756,  3.597872018814087,
         3.795919895172119
      ]
    }
  }
}
```

</details>
<details>
<summary>genshindb.talents('<b>mona'</b>)<b>.combat2</b></summary>

```js
{
  name: 'Mirror Reflection of Doom',
  info: 'Creates an illusory Phantom of Fate from coalesced waterspouts.\n' +
    '\n' +
    'The **Phantom** has the following special properties:\n' +
    '·Continuously taunts nearby opponents, attracting their fire.\n' +
    '·Continuously deals Hydro DMG to nearby opponents.\n' +
    '·When its duration expires, the Phantom explodes, dealing AoE Hydro DMG.\n' +
    '\n' +
    '**Hold**\n' +
    'Utilizes water currents to move backwards swiftly before conjuring a Phantom.\n' +
    '\n' +
    'Only one Phantom created by Mirror Reflection of Doom can exist at any time.',
  description: 'Skilled astrologers have always dreamed of using a phantom facsimile of themselves to ward off imminent ill fate, but Mona must be the first to make such a mockery of it in all of Teyvat.',
  attributes: {
    labels: [
      'DoT|{param1:F1P}',
      'Explosion DMG|{param2:P}',
      'CD|{param5:F1}s'
    ],
    parameters: {
      param1: [
        0.3199999928474426,
        0.3440000116825104,
        0.36800000071525574,
        0.4000000059604645,
        0.42399999499320984,
        0.4480000138282776,
        0.47999998927116394,
        0.5120000243186951,
        0.5440000295639038,
        0.5759999752044678,
        0.6079999804496765,
        0.6399999856948853,
        0.6800000071525574,
        0.7200000286102295,
        0.7599999904632568
      ],
      param2: [
        1.3279999494552612, 1.4276000261306763,
        1.5271999835968018,  1.659999966621399,
         1.759600043296814, 1.8592000007629395,
        1.9919999837875366,  2.124799966812134,
        2.2576000690460205,  2.390399932861328,
         2.523200035095215, 2.6559998989105225,
         2.822000026702881,   2.98799991607666,
        3.1540000438690186
      ],
      param5: [
        12, 12, 12, 12, 12, 12,
        12, 12, 12, 12, 12, 12,
        12, 12, 12
      ]
    }
  }
}
```

</details>
<details>
<summary>genshindb.talents('<b>mona'</b>)<b>.combatsp</b></summary>

```js
{
  name: 'Illusory Torrent',
  info: '**Alternate Sprint**\n' +
    "Mona cloaks herself within the water's flow, consuming Stamina to move rapidly.\n" +
    '\n' +
    'When under the effect of Illusory Torrent, Mona can move at high speed on water.\n' +
    'Applies the Wet status to nearby opponents when she reappears.',
  description: "This is something that Mona can do, but her teacher cannot. Well, but it's not as if her teacher would pursue any matter concerning Hydro Visions anyway...",
  attributes: {
    labels: [
      'Activation Stamina Consumption|{param1:F2}',
      'Stamina Drain|{param2:F2}/s'
    ],
    parameters: { param1: [ 10 ], param2: [ 15 ] }
  }
}
```

</details>
<details>
<summary>genshindb.talents('<b>mona'</b>)<b>.combat3</b></summary>

```js
{
  name: 'Stellaris Phantasm',
  info: 'Mona summons the sparkling waves and creates a reflection of the starry sky, applying the Illusory Bubble status to opponents in a large AoE.\n' +
    '\n' +
    '**Illusory Bubble**\n' +
    'Traps opponents inside a pocket of destiny and also makes them Wet. Renders weaker opponents immobile.\n' +
    'When an opponent affected by Illusory Bubble sustains DMG, it has the following effects:\n' +
    '·Applies an Omen to the opponent, which gives a DMG Bonus, also increasing the DMG of the attack that causes it.\n' +
    '·Removes the Illusory Bubble, dealing Hydro DMG in the process.\n' +
    '\n' +
    '**Omen**\n' +
    'During its duration, increases DMG taken by opponents.',
  description: 'It was from the time that gods first traced the lights in the heavens with their eyes that the notion of "fate" was born.',
  attributes: {
    labels: [
      'Illusory Bubble Duration|{param1:F1}s',
      'Illusory Bubble Explosion DMG|{param2:P}',
      'DMG Bonus|{param10:P}',
      'Omen Duration|{param4:F1}s',
      'CD|{param5:F1}s',
      'Energy Cost|{param6:I}'
    ],
    parameters: {
      param1: [
        8, 8, 8, 8, 8, 8,
        8, 8, 8, 8, 8, 8,
        8, 8, 8
      ],
      param2: [
         4.423999786376953, 4.755799770355225,
         5.087600231170654,  5.53000020980835,
         5.861800193786621, 6.193600177764893,
         6.636000156402588, 7.078400135040283,
        7.5208001136779785, 7.963200092315674,
         8.405599594116211, 8.847999572753906,
         9.401000022888184, 9.954000473022461,
        10.506999969482422
      ],
      param3: [
        -0.41999998688697815,
        -0.4399999976158142,
        -0.46000000834465027,
        -0.47999998927116394,
        -0.5,
        -0.5199999809265137,
        -0.5400000214576721,
        -0.5600000023841858,
        -0.5799999833106995,
        -0.6000000238418579,
        -0.6000000238418579,
        -0.6000000238418579,
        -0.6000000238418579,
        -0.6000000238418579,
        -0.6000000238418579
      ],
      param4: [
        4, 4, 4, 4.5, 4.5, 4.5,
        5, 5, 5,   5,   5,   5,
        5, 5, 5
      ],
      param5: [
        15, 15, 15, 15, 15, 15,
        15, 15, 15, 15, 15, 15,
        15, 15, 15
      ],
      param6: [
        60, 60, 60, 60, 60, 60,
        60, 60, 60, 60, 60, 60,
        60, 60, 60
      ],
      param10: [
        0.41999998688697815,  0.4399999976158142,
        0.46000000834465027, 0.47999998927116394,
                        0.5,  0.5199999809265137,
         0.5400000214576721,  0.5600000023841858,
         0.5799999833106995,  0.6000000238418579,
         0.6000000238418579,  0.6000000238418579,
         0.6000000238418579,  0.6000000238418579,
         0.6000000238418579
      ]
    }
  }
}
```

</details>

## genshindb.constellations(query[, opts])]

<details>
<summary>genshindb.constellations('<b>amber'</b>)</summary>

```js
{
  name: 'Amber',
  c1: {
    name: 'One Arrow to Rule Them All',
    effect: "Fires 2 arrows per **Aimed Shot**. The second arrow deals 20% of the first arrow's DMG."
  },
  c2: {
    name: 'Bunny Triggered',
    effect: "Baron Bunny, new and improved! Hitting Baron Bunny's foot with a fully-charged Aimed Shot manually detonates it.\n" +
      'Explosion via manual detonation deals 200% additional DMG.'
  },
  c3: {
    name: 'It Burns!',
    effect: 'Increases the Level of **Fiery Rain** by 3.\nMaximum upgrade level is 15.'
  },
  c4: {
    name: "It's Not Just Any Doll...",
    effect: "Decreases **Explosive Puppet**'s CD by 20%. Adds 1 additional charge."
  },
  c5: {
    name: "It's Baron Bunny!",
    effect: 'Increases the Level of **Explosive Puppet** by 3.\n' +
      'Maximum upgrade level is 15.'
  },
  c6: {
    name: 'Wildfire',
    effect: "**Fiery Rain** increases all party members' Movement SPD by 15% and ATK by 15% for 10s."
  },
  images: {
    c1: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_Ambor_01.png',
    c2: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_Ambor_02.png',
    c3: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_U_Ambor_02.png',
    c4: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_Ambor_03.png',
    c5: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_U_Ambor_01.png',
    c6: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_Ambor_04.png'
  }
}
```

</details>
<details>
<summary>genshindb.constellations('<b>childe'</b>)<b>.c3</b></summary>

```js
{
  name: 'Abyssal Mayhem: Vortex of Turmoil',
  effect: 'Increases the Level of **Foul Legacy: Raging Tide** by 3.\n' +
    'Maximum upgrade level is 15.'
}
```

</details>
<details>
<summary>genshindb.constellations('<b>traveler geo'</b>)</summary>

```js
{
  name: 'Traveler (Geo)',
  aliases: [ 'Geo Traveler', 'MC Geo', 'Geo MC' ],
  c1: {
    name: 'Invincible Stonewall',
    effect: 'Party members within the radius of **Wake of Earth** have their CRIT Rate increased by 10% and have increased resistance against interruption.'
  },
  c2: {
    name: 'Rockcore Meltdown',
    effect: 'When the meteorite created by **Starfell Sword** is destroyed, it will also explode, dealing additional AoE Geo DMG equal to the amount of damage dealt by Starfell Sword.'
  },
  c3: {
    name: 'Will of the Rock',
    effect: 'Increases the Level of **Wake of Earth** by 3.\n' +
      'Maximum upgrade level is 15.'
  },
  c4: {
    name: 'Reaction Force',
    effect: 'The shockwave triggered by **Wake of Earth** regenerates 5 Energy for every opponent hit.\n' +
      'A maximum of 25 Energy can be regenerated in this manner at any one time.'
  },
  c5: {
    name: 'Meteorite Impact',
    effect: 'Increases the Level of **Starfell Sword** by 3.\n' +
      'Maximum upgrade level is 15.'
  },
  c6: {
    name: 'Everlasting Boulder',
    effect: 'The barrier created by **Wake of Earth** lasts 5s longer.\n' +
      'The meteorite created by **Starfell Sword** lasts 10s longer.'
  },
  images: {
    c1: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_PlayerRock_01.png',
    c2: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_PlayerRock_02.png',
    c3: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_U_PlayerRock_02.png',
    c4: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_PlayerRock_03.png',
    c5: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_U_PlayerRock_01.png',
    c6: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/constellation_icon/UI_Talent_S_PlayerRock_04.png'
  }
}
```

</details>

## genshindb.weapons(query[, opts])]

<details>
<summary>genshindb.weapons('<b>names', { matchCategories: true }</b>)</summary>

```js
[
  'Alley Hunter',
  'Amber Bead',
  "Amos' Bow",
  "Apprentice's Notes",
  'Aquila Favonia',
  "Beginner's Protector",
  'Blackcliff Agate',
  'Blackcliff Longsword',
  'Blackcliff Pole',
  'Blackcliff Slasher',
  'Blackcliff Warbow',
  'Black Tassel',
  'Bloodtainted Greatsword',
  'Compound Bow',
  'Cool Steel',
  'Crescent Pike',
  'Dark Iron Sword',
  'Deathmatch',
  'Debate Club',
  "Dragon's Bane",
  'Dragonspine Spear',
  'Dull Blade',
  'Ebony Bow',
  'Elegy for the End',
  'Emerald Orb',
  'Eye of Perception',
  'Favonius Codex',
  'Favonius Greatsword',
  'Favonius Lance',
  'Favonius Sword',
  'Favonius Warbow',
  'Ferrous Shadow',
  'Festering Desire',
  'Fillet Blade',
  'Frostbearer',
  'Halberd',
  'Harbinger of Dawn',
  "Hunter's Bow",
  'Iron Point',
  'Iron Sting',
  "Lion's Roar",
  'Lithic Blade',
  'Lithic Spear',
  'Lost Prayer to the Sacred Winds',
  'Magic Guide',
  'Mappa Mare',
  'Memory of Dust',
  'Messenger',
  "Old Merc's Pal",
  'Otherworldly Story',
  'Pocket Grimoire',
  'Primordial Jade Cutter',
  'Primordial Jade Winged-Spear',
  'Prototype Amber',
  'Prototype Archaic',
  'Prototype Crescent',
  'Prototype Rancour',
  'Prototype Starglitter',
  'Quartz',
  'Rainslasher',
  'Raven Bow',
  'Recurve Bow',
  'Royal Bow',
  'Royal Greatsword',
  'Royal Grimoire',
  'Royal Longsword',
  'Royal Spear',
  'Rust',
  'Sacrificial Bow',
  'Sacrificial Fragments',
  'Sacrificial Greatsword',
  'Sacrificial Sword',
  "Seasoned Hunter's Bow",
  'Serpent Spine',
  "Sharpshooter's Oath",
  'Silver Sword',
  'Skyrider Greatsword',
  'Skyrider Sword',
  'Skyward Atlas',
  'Skyward Blade',
  'Skyward Harp',
  'Skyward Pride',
  'Skyward Spine',
  'Slingshot',
  'Snow-Tombed Starsilver',
  'Solar Pearl',
  'Song of Broken Pines',
  'Staff of Homa',
  'Summit Shaper',
  'Sword of Descension',
  'The Alley Flash',
  'The Bell',
  'The Black Sword',
  'The Flagstaff',
  'The Flute',
  'The Stringless',
  'The Unforged',
  'The Viridescent Hunt',
  'The Widsith',
  'Thrilling Tales of Dragon Slayers',
  ... 10 more items
]
```

</details>
<details>
<summary>genshindb.weapons('<b>lost prayers'</b>)</summary>

```js
{
  name: 'Lost Prayer to the Sacred Winds',
  description: 'An educational tome written by anonymous early inhabitants who worshiped the wind. It has been blessed by the wind for its faithfulness and influence over the millennia.',
  weapontype: 'Catalyst',
  rarity: '5',
  baseatk: 46,
  substat: 'CRIT Rate',
  subvalue: '7.2',
  effectname: 'Boundless Blessing',
  effect: 'Increases Movement SPD by 10%. When in battle, gain a {0} Elemental DMG Bonus every 4s. Max 4 stacks. Lasts until the character falls or leaves combat.',
  r1: [ '8%' ],
  r2: [ '10%' ],
  r3: [ '12%' ],
  r4: [ '14%' ],
  r5: [ '16%' ],
  weaponmaterialtype: 'Dandelion Gladiator',
  images: {
    image: 'https://static.wikia.nocookie.net/gensin-impact/images/9/98/Weapon_Lost_Prayer_to_the_Sacred_Winds.png',
    icon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_EquipIcon_Catalyst_Fourwinds.png',
    awakenicon: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_EquipIcon_Catalyst_Fourwinds_Awaken.png'
  },
  url: {
    fandom: 'https://genshin-impact.fandom.com/wiki/Lost_Prayer_to_the_Sacred_Winds'
  },
  stats: [Function (anonymous)]
}
```

</details>
<details>
<summary>genshindb.weapons('<b>decarabian', { matchCategories: true }</b>)</summary>

```js
[
  "Apprentice's Notes",
  'Aquila Favonia',
  'Cool Steel',
  'Dull Blade',
  'Favonius Codex',
  'Favonius Sword',
  'Ferrous Shadow',
  'Magic Guide',
  'Pocket Grimoire',
  'Raven Bow',
  'Royal Grimoire',
  'Royal Longsword',
  'Silver Sword',
  'Snow-Tombed Starsilver',
  'The Bell',
  'The Stringless',
  'The Viridescent Hunt'
]
```

</details>
<details>
<summary>genshindb.weapons('<b>dull blade'</b>)<b>.stats(49)</b></summary>

```js
{ level: 49, ascension: 2, attack: 127.972232961788, specialized: 0 }
```

</details>
<details>
<summary>genshindb.weapons('<b>sac sword'</b>)<b>.stats(80, '+')</b></summary>

```js
{
  level: 80,
  ascension: 6,
  attack: 426.5607374033825,
  specialized: 0.5586652674078749
}
```

</details>
<details>
<summary>genshindb.weapons('<b>wolf grave'</b>)<b>.stats(90)</b></summary>

```js
{
  level: 90,
  ascension: 6,
  attack: 608.074622109998,
  specialized: 0.49615199803817234
}
```

</details>

## genshindb.weaponmaterialtypes(query[, opts])]

<details>
<summary>genshindb.weaponmaterialtypes('<b>chains'</b>)</summary>

```js
{
  name: 'Dandelion Gladiator',
  '2starname': 'Fetters of the Dandelion Gladiator',
  '3starname': 'Chains of the Dandelion Gladiator',
  '4starname': 'Shackles of the Dandelion Gladiator',
  '5starname': 'Dream of the Dandelion Gladiator',
  day: [ 'Wednesday', 'Saturday', 'Sunday' ],
  location: 'Wolvendom',
  region: 'Mondstadt',
  domainofforgery: 'Cecilia Garden',
  images: undefined
}
```

</details>
<details>
<summary>genshindb.weaponmaterialtypes('<b>fri', { matchCategories: true }</b>)</summary>

```js
[ 'Boreal Wolf', 'Mist Veiled Elixir' ]
```

</details>

## genshindb.talentmaterialtypes(query[, opts])]

<details>
<summary>genshindb.talentmaterialtypes('<b>ballad'</b>)</summary>

```js
{
  name: 'Ballad',
  '2starname': 'Teachings of "Ballad"',
  '3starname': 'Guide of "Ballad"',
  '4starname': 'Philosophies of "Ballad"',
  day: [ 'Wednesday', 'Saturday', 'Sunday' ],
  location: 'Springvale',
  region: 'Mondstadt',
  domainofmastery: 'Forsaken Rift',
  images: undefined
}
```

</details>
<details>
<summary>genshindb.talentmaterialtypes('<b>satur', { matchCategories: true }</b>)</summary>

```js
[ 'Ballad', 'Gold' ]
```

</details>

## genshindb.artifacts(query[, opts])]

<details>
<summary>genshindb.artifacts('<b>flame'</b>)</summary>

```js
{
  name: 'Pale Flame',
  rarity: [ '4', '5' ],
  '2pc': 'Physical DMG is increased by 25%.',
  '4pc': 'When an Elemental Skill hits an opponent, ATK is increased by 9% for 7s. This effect stacks up to 2 times and can be triggered once every 0.3s. Once 2 stacks are reached, the 2-set effect is increased by 100%.',
  flower: {
    name: 'Stainless Bloom',
    relictype: 'Flower of Life',
    description: 'A hard, blue artificial flower. Its petals shall never wither, nor shall its colors fade.'
  },
  plume: {
    name: "Wise Doctor's Pinion",
    relictype: 'Plume of Death',
    description: 'An ominous pinion with edges of unsurpassed keenness. Perhaps it represents an unnaturally uninhibited nature.'
  },
  sands: {
    name: 'Moment of Cessation',
    relictype: 'Sands of Eon',
    description: 'A pocket watch with a cover that cannot be opened. Yet it ticks and tocks away, following the inexorable flow of time.'
  },
  goblet: {
    name: 'Surpassing Cup',
    relictype: 'Goblet of Eonothem',
    description: 'An intricately-made cup. Its appearance betrays nothing of its age to an observer.'
  },
  circlet: {
    name: 'Mocking Mask',
    relictype: 'Circlet of Logos',
    description: "A mask that covers the face, hiding one's expression from others."
  },
  images: {
    flower: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_RelicIcon_15018_4.png',
    plume: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_RelicIcon_15018_2.png',
    sands: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_RelicIcon_15018_5.png',
    goblet: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_RelicIcon_15018_1.png',
    circlet: 'https://upload-os-bbs.mihoyo.com/game_record/genshin/equip/UI_RelicIcon_15018_3.png'
  },
  url: { fandom: 'https://genshin-impact.fandom.com/wiki/Pale_Flame' }
}
```

</details>
<details>
<summary>genshindb.artifacts('<b>5', { matchCategories: true }</b>)</summary>

```js
[
  'Archaic Petra',
  'Blizzard Strayer',
  'Bloodstained Chivalry',
  'Crimson Witch of Flames',
  "Gladiator's Finale",
  'Heart of Depth',
  'Lavawalker',
  'Maiden Beloved',
  'Noblesse Oblige',
  'Pale Flame',
  'Retracing Bolide',
  'Tenacity of the Millelith',
  'Thundering Fury',
  'Thundersoother',
  'Viridescent Venerer',
  "Wanderer's Troupe"
]
```

</details>
<details>
<summary>genshindb.artifacts('<b>noblesse'</b>)<b>['2pc']</b></summary>

```js
'Elemental Burst DMG +20%'
```

</details>

## genshindb.foods(query[, opts])]

<details>
<summary>genshindb.foods('<b>temptation'</b>)</summary>

```js
{
  name: "Adeptus' Temptation",
  rarity: 5,
  foodtype: 'NORMAL',
  foodfilter: 'ATK-Boosting Dish',
  foodcategory: 'Atk_Add',
  effect: "Increases all party members' ATK by 260–372 and CRIT Rate by 8–12% for 300s.\n" +
    'In Co-Op Mode, this effect only applies to your own character(s).',
  description: 'A complex, famous type of Liyue cuisine, in which specially selected ingredients are submerged and slowly boiled in soup stock. The recipe scribbled from memory alone was enough to urge the adepti to once again return to the world of men.',
  suspicious: {
    effect: "Increases all party members' ATK by 260 and CRIT Rate by 8% for 300s. In Co-Op Mode, this effect only applies to your own character(s).",
    description: "A complex, famous type of Liyue cuisine. Without having mastered the art of simmering, the resulting stew-like dish has a salty, fishy taste. But, just considering the costly ingredients will be enough to keep you going until the pot's empty."
  },
  normal: {
    effect: "Increases all party members' ATK by 316 and CRIT Rate by 10% for 300s. In Co-Op Mode, this effect only applies to your own character(s).",
    description: 'A complex, famous type of Liyue cuisine, in which specially selected ingredients are submerged and slowly boiled in soup stock. The recipe scribbled from memory alone was enough to urge the adepti to once again return to the world of men.'
  },
  delicious: {
    effect: "Increases all party members' ATK by 372 and CRIT Rate by 12% for 300s. In Co-Op Mode, this effect only applies to your own character(s).",
    description: "A complex, famous type of Liyue cuisine. This dish is a rare and exquisite mix of both land and sea, combining countless delicious delicacies in one flavor-filled pot. Each mouthful is a moment to remember — it's even irresistible enough to entice the adepti down from their celestial abode."
  },
  ingredients: [
    { name: 'Ham', count: 4 },
    { name: 'Crab', count: 3 },
    { name: 'Shrimp Meat', count: 3 },
    { name: 'Matsutake', count: 3 }
  ],
  images: {},
  url: {
    fandom: "https://genshin-impact.fandom.com/wiki/Adeptus'_Temptation"
  }
}
```

</details>
<details>
<summary>genshindb.foods('<b>4', { matchCategories: true }</b>)</summary>

```js
[
  'Golden Crab',
  'Golden Fried Chicken',
  'Jade Parcels',
  'Moon Pie',
  'Stormcrest Pie',
  'Tianshu Meat'
]
```

</details>
<details>
<summary>genshindb.foods('<b>def', { matchCategories: true }</b>)</summary>

```js
[
  'A Prize Catch',
  'Calla Lily Seafood Soup',
  "Fisherman's Toast",
  'Fish-Flavored Toast',
  'Golden Crab',
  'Jewelry Soup',
  'Lotus Flower Crisp',
  'Moon Pie',
  'Stormcrest Pie',
  'Sunshine Sprat',
  'Triple-Layered Consommé',
  'Woodland Dream'
]
```

</details>
<details>
<summary>genshindb.foods('<b>cabbage', { matchCategories: true }</b>)</summary>

```js
[
  'Crab, Ham & Veggie Bake',
  'Der Weisheit Letzter Schluss (Life)',
  'Golden Chicken Burger',
  'Invigorating Pizza',
  'Jade Parcels',
  'Mushroom Pizza',
  'Northern Smoked Chicken',
  'Nutritious Meal (V.593)',
  'Qingce Stir Fry',
  'Satisfying Salad'
]
```

</details>
<details>
<summary>genshindb.foods('<b>diluc', { matchAliases: true }</b>)</summary>

```js
{
  name: '"Once Upon a Time in Mondstadt"',
  rarity: 3,
  foodtype: 'SPECIALTY',
  foodfilter: 'ATK-Boosting Dish',
  foodcategory: 'Atk_CritRate',
  effect: "Increases all party members' CRIT Rate by 20% and CRIT DMG by 20% for 300s. In Co-Op Mode, this effect only applies to your own character(s)",
  description: "Diluc's specialty. Feast your eyes and then your stomach upon this delicacy as the soft ribs melt in your mouth. Who knew Diluc was able to cook this well?",
  basedish: `"Pile 'Em Up"`,
  character: 'Diluc',
  ingredients: [
    { name: 'Raw Meat', count: 3 },
    { name: 'Potato', count: 3 },
    { name: 'Small Lamp Grass', count: 1 },
    { name: 'Cheese', count: 1 }
  ],
  images: {},
  url: {
    fandom: 'https://genshin-impact.fandom.com/wiki/"Once_Upon_a_Time_in_Mondstadt"'
  }
}
```

</details>

## genshindb.elements(query[, opts])]


## genshindb.rarity(query[, opts])]

