## index
- タイトルロゴ下に`アイギス・アークってなに？`リンク（about.html）を追加したい。
- リセットボタンより下に小さく、`不具合報告はサイト製作者X(https://x.com/Mimmy_zeta001)まで`を表示したい



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
