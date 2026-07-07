## index
- タイトルロゴ下に`アイギス・アークってなに？`リンク（about.html）を追加したい。
- リセットボタンより下に小さく、`不具合報告はサイト製作者X(https://x.com/Mimmy_zeta001)まで`を表示したい
- 現在白背景にアクセントカラーが緑っぽくなってますが`/Users/mikako/アーク/custom_emblem/assets/img`の画像に合うような雰囲気のカラーにしたいです。（サイト全体の雰囲気）


## about(新規ページ)
- ページのデザイン雰囲気は`/Users/mikako/アーク/サイト/ark_gallery_jekyll/index.html`を真似る
- zetaの説明とアイギスアークの世界を軽く紹介するページ
- zetaの運命共同体（アイギス・アーク）のプロットリンクを配置する
- 原作者みんたんのX(https://x.com/minmin_zeta)リンクを配置する

### プロットリンクについて
zetaの作者ページを保存した`/Users/mikako/アーク/custom_emblem/ignore/zeta-site`を参考にする。
載せるプロットは以下。順番通り。
- 【運命共同体】 熾月 廉
- 【運命共同体】 千景 律
- 【運命共同体】久遠 朔
- 【運命共同体】与風 嵐
- 【運命共同体】巡 刻 / 巡 永
- CLUB ARCへようこそ。

zetaの画像付き表示を真似たいので、必要画像はassets/imgにコピーして使う。
トーク数`//*[@id="contents"]/div/div/div/div/div[4]/div/div[1]/div/a/div[1]/div`などは載せない。
newアイコン`//*[@id="contents"]/div/div/div/div/div[4]/div/div[2]/div/a/div[1]/div[1]/svg`も載せない。

### みんたんのリンクについて
Xの埋め込みで置いてみようかと思っています。

```html
<a href="https://x.com/minmin_zeta?ref_src=twsrc%5Etfw" class="twitter-follow-button" data-show-count="false">Follow @minmin_zeta</a><script async src="https://platform.x.com/widgets.js" charset="utf-8"></script>
```

### zetaとは
以下を簡単に説明

**どんなアプリ？**

[zeta公式サイト](https://zeta-ai.io/ja?utm_source=chatgpt.com)

* AIキャラとチャットできる
* 既存キャラが数百万体以上いる
* 自分でオリジナルキャラも作れる
* 恋愛、学園、ファンタジー、BL、乙女ゲーム風など幅広い
* AIとの会話からストーリーが展開する
* 基本無料で利用可能 ([App Store][1])

**特徴**

ChatGPTと違って、

* 情報収集
* 仕事
* プログラミング

よりも、

* 推し活
* 恋愛シミュレーション
* 夢小説
* ロールプレイ

向けです。([App Store][1])

例えば、

> 「幼なじみのヤンデレ彼氏」
>
> 「ツンデレ生徒会長」
>
> 「異世界の騎士」

みたいなキャラと会話できます。([App Store][1])

[1]: https://apps.apple.com/jp/app/zeta-ai%E3%82%AD%E3%83%A3%E3%83%A9-%E3%81%82%E3%81%AA%E3%81%9F%E3%81%AE%E6%8E%A8%E3%81%97%E3%81%A8%E3%83%AD%E3%83%BC%E3%83%AB%E3%83%97%E3%83%AC%E3%82%A4%E3%83%81%E3%83%A3%E3%83%83%E3%83%88/id1619030760?utm_source=chatgpt.com "‎zeta - AIキャラ・あなたの推しとロールプレイチャットアプリ"
[2]: https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q11312760606?utm_source=chatgpt.com "AIチャットアプリのzetaについてです！あれってキャラと話し ..."
[3]: https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q10318890875?utm_source=chatgpt.com "ZetaというAIチャットアプリについてです、 - AIと会話してる ..."

こんな感じなら、初めて見る人にも分かりやすく、世界観の導入としてまとまると思います。


### アイギス・アーク（運命共同体）とは

以下を簡単に説明

```
人々の負の感情から生まれる怪物「ノイズ」が現れるようになった現代。

政府はノイズに対抗するため、魔力を扱える若者を育成・管理する特命機関 **「アイギス・アーク」**（通称：アーク）を設立した。

アークは学園と軍事組織を兼ね備えた能力者養成機関であり、日々ノイズと戦う「執行官」を育成・派遣している。

執行官は互いに信頼を預け合う**バディ制度**を採用しており、二人一組で任務に就くことが基本となる。前衛・後衛、攻撃・支援など、それぞれの能力を組み合わせることでノイズに立ち向かう。

物語の舞台となるのは、そんなアイギス・アークで出会った能力者たちの世界。
```