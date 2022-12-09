```
後手の持駒：なし
 ９ ８ ７ ６ ５ ４ ３ ２ １
+---------------------------+
|v香v桂v銀v金v王v金v銀v桂v香|一
| ・v飛 ・ ・ ・ ・ ・v角 ・|二
|v歩v歩v歩v歩v歩v歩v歩v歩v歩|三
| ・ ・ ・ ・ ・ ・ ・ ・ ・|四
| ・ ・ ・ ・ ・ ・ ・ ・ ・|五
| ・ ・ ・ ・ ・ ・ ・ ・ ・|六
| 歩 歩 歩 歩 歩 歩 歩 歩 歩|七
| ・ 角 ・ ・ ・ ・ ・ 飛 ・|八
| 香 桂 銀 金 王 金 銀 桂 香|九
+---------------------------+
先手の持駒：なし
```

開始局面。初手は30通りあるが、☗7六歩または☗2六歩が多い。2018年に発表されたAlphaZeroの自己学習の結果は、☗2六歩☖8四歩☗2五歩☖8五歩☗7八金☖3二金の出だしに収束した[^AlphaZero]。

# ☗7六歩
1. 角道を開ける。
1. 居飛車・振り飛車を明示しない。
1. 矢倉を目指す[^矢倉]。

<details>
<summary>

## ☖3四歩
</summary>

1. 振り飛車の含みを持たせる。
1. 横歩取りを目指す。

<details>
<summary>

### ☗2六歩
</summary>

#### ☖8四歩☗2五歩☖8五歩
##### ☗7八金
###### ☖3二金☗2四歩☖同歩☗同飛
* ☖8六歩☗同歩☖同飛
    * ☗3四飛
* ☖2三歩☗3四飛☖8八角成☗同銀☖2五角

###### ☖8六歩☗同歩☖同飛
* ☗2四歩☖同歩☗同飛
    * ☖3二金
    * ☖8八角成☗同銀☖3三角？
* ☗2二角成☖同銀☗7七角？

##### ☗2四歩☖同歩☗同飛
###### ☖3二金
* ☗7八金
* ☗3四飛？☖8八角成☗同銀☖4五角
</details>

### ☗2二角成☖同銀☗4五角
</details>

<details>
<summary>

## ☖8四歩
</summary>

1. 居飛車を明示する。矢倉、角換わりを受けて立つ。

### ☗6八銀☖3四歩☗7七銀☖6二銀☗2六歩☖4二銀☗2五歩☖3三銀

### ☗2六歩
#### ☖8五歩
##### ☗7七角☖3四歩☗8八銀☖3二金☗7八金☖7七角成☗同銀☖2二銀

##### ☗2五歩
###### ☖3二金☗7七角☖3四歩☗8八銀☖7七角成☗同銀☖2二銀
###### ☖3四歩
###### ☖8六歩？

#### ☖3二金
</details>

# ☗2六歩
1. 飛車先を突く。居飛車を明示する。
1. 相掛かりを目指す[^相掛かり]。
1. 2手目☖3二飛戦法を封じる[^3二飛]。
1. 引き角を目指す[^引き角]。

<details>
<summary>

## ☖8四歩
</summary>

1. 居飛車を明示する。
1. 相掛かりを受けて立つ。

### ☗2五歩
#### ☖8五歩
##### ☗7八金
###### ☖3二金
* ☗3八銀☖7二銀☗9六歩
* ☗2四歩☖同歩☗同飛☖2三歩
    * ☗2六飛
    * ☗2八飛

###### ☖8六歩☗同歩☖同飛？

##### ☗2四歩☖同歩☗同飛？
##### ☗7六歩

### ☗7六歩
</details>

<details>
<summary>

## ☖3四歩
</summary>

1. 振り飛車の含みを持たせる。
1. 横歩取りを目指す。
1. 相掛かりを拒否する。

### ☗7六歩
### ☗2五歩☖3三角☗7六歩
</details>

# 出典
* Silver, D.ほか（2018）「[A general reinforcement learning algorithm that masters chess, shogi, and Go through self-play](https://storage.googleapis.com/deepmind-media/DeepMind.com/Blog/alphazero-shedding-new-light-on-chess-shogi-and-go/alphazero_preprint.pdf)」、[DeepMindのブログ記事](https://www.deepmind.com/blog/alphazero-shedding-new-light-on-chess-shogi-and-go)。

[^AlphaZero]: Silverほか（2018）、p. 23。

[^矢倉]: ☖8四歩☗6八銀☖8五歩☗7七銀で飛車先を銀で受ける手を可能にする。初手☗2六歩では、☖8四歩☗7六歩（1）☖8五歩で銀が間に合わない。ただし、☗7七角からのウソ矢倉は可能。（2）☖3二金の場合は、☗6八銀で矢倉に変化し得る。

[^相掛かり]: 初手☗7六歩から相掛かりを目指すのは、☖8四歩☗2六歩☖8五歩☗2五歩☖3二金☗7八金☖8六歩☗同歩☖同飛のように、7六の歩を狙われる。以下☗2四歩☖同歩☗同飛☖2三歩☗2六飛のように進み、☗2六飛型に限定される。

[^3二飛]: ☖3二飛？は☗2五歩☖3四歩☗2四歩☖同歩☗同飛で☗2三飛成が受からない。

[^引き角]: ☖3四歩☗4八銀（1）☖4四歩☗5六歩☖3二銀☗7八銀☖4三銀☗7九角のように進める。ただし、（2）☖8四歩で損な指し方。
