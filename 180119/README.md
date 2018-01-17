# KEGG データベースの使い方

東京農業大学　生命科学部分子　微生物学科
Department of Molecular Microbiology, Faculty of Life Sciences, Tokyo University of Agriculture

志波　優
Yuh Shiwa, PhD
youyuh48@gmail.com

Update: January 19, 2018

## KEGGとは？

>KEGG はゲノムや分子レベルの情報から細胞、個体、エコシステムといった生命システムの機能や有用性を理解するためのリソースです。生命システムのコンピュータ表現として、遺伝子やタンパク質（ゲノム情報）と化合物など（ケミカル情報）の分子部品の情報を、分子間の相互作用・反応・関係ネットワーク（システム情報）の知識で統合した生命システム情報統合データベースです。さらに生体システムのゆらぎとして疾患・医薬品情報（ヘルス情報）も統合されています。出典：[KEGG の概要](http://www.genome.jp/kegg/kegg1a_ja.html)

![](http://www.kegg.jp/kegg/docs/fig/kegg_overview_ja.gif)
> 画像出典：[KEGG の概要](http://www.genome.jp/kegg/kegg1a_ja.html)

## ビタミンC

>ヒトやサル、モルモットは体内でビタミンCを合成できません。その理由は、ビタミンC生合成経路の最後に位置する酵素（GLO：グロノ-γ-ラクトン酸化酵素）に遺伝子変異があるためです（図4）。しかし、マウスはこの酵素（GLO）に遺伝子変異がないため、体内で充分量のビタミンCを合成できます。ビタミンとは、本来、身体の中で作れない物質ですから、マウスにとってビタミンCはビタミンではないのです。出典：[ヒトは体内でビタミンCを合成できない](http://www.vit-c.jp/vitaminc/vc-02.html)

![](http://www.vit-c.jp/vitaminc/img/pict_104.gif)
> 画像出典：[ヒトは体内でビタミンCを合成できない](http://www.vit-c.jp/vitaminc/vc-02.html)

## KEGG Pathway の使い方

### 遺伝子名・酵素名から検索

* [KEGG](http://www.genome.jp/kegg/) のページを開く
* トップページの検索窓に `L-gulonolactone oxidase` を入力してSearchをクリック
* KEGG ORTHOLOGY に表示された `K00103` をクリック
* Pathway に表示された `ko00053` をクリック
* ![](https://user-images.githubusercontent.com/27807944/34324596-18fdb730-e8bc-11e7-9e57-968fe964ee16.png)
  - 文献情報から作成されたリファレンスパスウェイが表示される
  - 図中の○が代謝産物、□が酵素
  - 赤枠の酵素が検索した`L-gulonolactone oxidase`
* ヒトがこのパスウェイで持っている遺伝子を重ねて表示させる
  - `Reference pathway (KO)`をクリックし、`Homo sapiens (human)`を選択し、Goをクリック
  - 遺伝子`1.1.3.8`に色が付いていないため、当該遺伝子がヒトゲノムに無いことがわかる
* マウスがこのパスウェイで持っている遺伝子を重ねて表示させる
  - `Reference pathway (KO)`をクリックし、`Mus musculus (mouse)`を選択し、Goをクリック
  - 遺伝子`1.1.3.8`に緑色が付いており、当該遺伝子がマウスゲノムに存在することがわかる
  - 遺伝子`1.1.3.8`をクリックすると、当該遺伝子情報が表示される

### 化合物名から検索

* トップページの検索窓に `Ascorbic acid` を入力してSearchをクリック
* KEGG COMPOUND に表示された `C00072` をクリックすると、当該化合物情報が表示される
* Pathway に表示された `map00053` をクリックすると、パスウェイ上で当該化合物が赤丸で表示される
  - この化合物が先ほどの遺伝子`1.1.3.8`の代謝産物の一つであることがわかる
* COMPOUND ページに戻って、Module に表示された `M00129` をクリックする
  - 動物でのアスコルビン酸の生合成に関わるモジュール（遺伝子・反応・化合物のセット）が表示される
  - 左列：KO遺伝子（KEGGのオーソログ遺伝子ID）
  - 右列：化合物と反応
  - `Reference module (KO)`をクリックすると、当該合成系を持つ生物名が表示される

### 疾患名から検索

* トップページ -> KEGG DISEASE -> 右上の`Japanese`をクリック
* 検索窓に`壊血病`を入力して検索をクリック
* 検索結果に表示された`H01580`をクリックすると、当該疾患に関する情報が表示される

***

## 課題

ビタミン欠乏症について調査する。
下記の内容をレポートにまとめること（Wordファイル）
時間が余ったら、もう一つの欠乏症も調査すること（途中で終わっても良い）

- 選んだビタミン欠乏症の概要は？
  - トップページ -> KEGG DISEASE -> 右上の`Japanese`をクリック
  - 検索窓に`ビタミン　欠乏`を入力して検索をクリック
  - 興味あるビタミン欠乏症をクリック（ビタミンC以外）
  - 当該疾患の概要をレポートに記載
- そのビタミンの化合物名は？
  - `ビタミンC`に対する`Ascorbic acid`のような化合物名
  - 疾患のページから戻り、疾患一覧治療薬欄の`DR:Dxxxxx`をクリックすると薬剤ページ(DRUG)に飛ぶ
  - Simcompの`Neighbor`をクリックすると構造が類似している化合物が表示される
  - scoreが最も高い`C`で始まるIDをクリックすると化合物ページ(COMPOUND)に飛ぶ
  - Nameに表示された化合物名、Entry欄に表示されたIDをレポートに記載
  - Structure欄に表示された化合物の構造式の画像をコピーしてレポートに貼る
- その化合物を合成できる代謝系（モジュール）をもつ生物は？
  - 化合物ページ(COMPOUND)のModule欄の`〜 biosynthesis`と記載されているIDをクリック
  - `Reference module (KO)`をクリックすると、当該合成系を持つ生物名が表示される
  - 生物名を３つレポートに記載、学名だけでなく日本語名も併記する
- その化合物をヒトの小腸の上皮細胞に取り込む膜タンパク質の名前は？
  - ページを戻って`COMPOUND`を表示させる
  - Pathwayの `map04977` Vitamin digestion and absorption をクリック
  - その化合物を取り込むトランスポーターをクリック（図中の上皮のマップ中の赤丸が通過する）
  - `Entry`, `Name`, `Definition` をレポートに記載

***

## 参考情報

* [KEGG/GenomeNetの利用法](http://motdb.dbcls.jp/?plugin=attach&pcmd=open&file=KEGG_2013_11.pdf&refer=AJACS43)
* [創薬に向けた KEGG パスウェイ解析](http://hinv.jp/pdf/20120120/KEGG_pathway.pdf)
* [パスウェイデータベースの紹介とKEGG PATHWAYの使い方](http://togotv.dbcls.jp/ajacs2016003.html)

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">クリエイティブ・コモンズ 表示 4.0 国際 ライセンス</a>の下に提供されています。
